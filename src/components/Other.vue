<template>
    <div class="other-works-container">
        <h3>My other works</h3>
        <div class="grid">
            <div v-for="(project, i) in otherWorks" :key="project.id" :class="`grid-${i % 6}`">
                <img :src="project.img" :alt="project.alt">
            </div>
        </div>
        <div class="other-works-container-btn">
            <a href="#" target="_blank">See more</a>
        </div>
    </div>
</template>
<script>
export default {
    props:{
        otherWorks : Array
    }
}
</script>
<style lang="scss" scoped>

.other-works-container{
    width: 80%;
    margin: 3rem auto 5rem;

    h3{
        font-size: 4rem;
        font-weight: 600;
        letter-spacing: -0.2rem;
    }

    .grid{
        display: grid;
        grid-gap: 1rem;
        margin-top: 3rem;
        grid-template-columns: repeat(4, 1fr);

        img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }

        &-0{
            background: darkorange;
            height: 100%;
        }

        &-2{
            grid-column-start: 3;
            grid-column-end: 5;
        }

        &-3{
            background: linear-gradient(302.04deg, #2E62EC 0%, #58A3DF 100%);
            grid-column-start: 1;
            grid-column-end: 3;
        }

        &-5{
            background-color: darkgray;
        }
    }

    &-btn{
        margin: auto;
        margin-top: 3rem;
        width: 11.25rem;
        height: 3rem;
        display: flex;
        justify-content: center;
        align-items: center;
        background-color: #6cd1f3;

        a{
            width: 100%;
            height: 100%;
            display: flex;
            justify-content: center;
            align-items: center;
            text-decoration: none;
            font-weight: 600;
            color: white;
        }
    }

}

</style>