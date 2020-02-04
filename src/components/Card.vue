<template>
    <div class="card-container" :class="{'card-container--featured': isFeatured}">
        <div class="card-container-txt">
            <div class="card-container-txt-title">
                {{ title }}
            </div>
            <div class="card-container-txt-subtitle">
                {{ subtitle }}
            </div>
            <div class="card-container-txt-excerpt">
                {{ excerpt }}
            </div>
            <div class="card-container-txt-btn">
                <a href="#" target="_blank">{{ link }}</a>
            </div>
        </div>
        <div class="card-container-img">
            <img :src="thumbnail" alt="illustration projet">
        </div>
    </div>
</template>

<script>
export default {
    props:{
        id : Number,
        title : String,
        subtitle : String,
        excerpt : String,
        thumbnail : String,
        link : String,
        isFeatured: {
            type: Boolean,
            default: false
        }
    }
}
</script>

<style lang="scss" scoped>

.card-container{
    // width: 50rem;
    width: 50%;
    // height: 18rem;
    margin: 6rem auto;
    background-color: white;
    display: flex;
    box-shadow: 0px 9px 15px 4px rgba(173, 183, 189, 0.08);


    &--featured {
        margin: 10rem auto;
        box-shadow: none;
        width: 50%;
    }

    &:nth-child(even) {
        flex-direction: row-reverse;
    }

    &-txt{
        width: 50%;
        padding: 3rem 2rem;

        &-title{
            font-size: 1.3rem;
            font-weight: 700;
        }

        &-subtitle{
            padding: 0.6rem 0 1rem 0;
            color: darkgrey;
        }

        &-excerpt{
            line-height: 1.3;
        }

        &-btn{
            margin-top: 1.5rem;
            a{
                text-decoration: none;
                color: #6cd1f3;
                font-weight: 600;

                &::after{
                    content: "--→";
                    color: #6cd1f3;
                    margin-left: 0.5rem;
                }
            }
        }
    }

    &-img{
        width: 50%;

        img{
            width: 100%;
        }
    }

}
</style>