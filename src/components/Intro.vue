<template>
    <div class="intro">
        <div class="intro-title">
            <div>Paris based digital designer</div>
        </div>
        <div class="intro-text">
            <div class="intro-text-up">
                <p>Bonjour ! I’m Nemo Fazakerley, a digital designer from and living in Paris. I’m currently studying at HETIC and am available for freelance work.</p>
            </div>
            <div class="intro-text-down">
                <p>I am actively looking for a 5 month internship in Berlin, Warsaw or Budapest. Feel free to conctact me !</p>
            </div>
            <div class="intro-text-contact-btn">
                <a href="#" target="_blank">
                    Contact me
                </a>
            </div>
        </div>
    </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>

.intro{
    height: 27rem;
    width: 80%;
    margin: auto;
    display: flex;
    justify-content: space-evenly;
    color: white;


    &-title{
        // width: 30rem;
        font-size: 3.75rem;
        font-weight: 600;
        display: flex;
        // align-items: center;
        // border-top: solid thin white;
        padding-top: 2rem;

        // &::before{
        //     content: '';
        //     position: absolute;
        //     top: 32%;
        //     transform: translateY(-32%);
        //     background-color: white;
        //     border-radius: 2px;
        //     width: 29rem;
        //     height: 0.05rem; //calc(100% - 0px)
        // }
    }

    &-text{
        // width: 28.7rem;
        padding-top: 2rem;
        line-height: 1.5;
        display: flex;
        // align-items: center;
        flex-direction: column;
        // border-top: solid thin white;

        // &::before{
        //     content: '';
        //     position: absolute;
        //     top: 32%;
        //     transform: translateY(-32%);
        //     background-color: white;
        //     border-radius: 2px;
        //     width: 29rem;
        //     height: 0.05rem; //calc(100% - 0px)
        // }

        &-up{
            font-weight: 200;
            // width: 29rem;
        }

        &-down{
            font-weight: 600;
            margin: 2rem 0;
        }

        &-contact-btn{
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
}


</style>