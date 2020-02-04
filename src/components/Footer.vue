<template>
  <footer>
    <div class="footer-container">
      <div class="footer-container-about">
        <div class="footer-container-about-title">
          About me
        </div>
        <div class="footer-container-about-txt">
          <div class="footer-container-about-txt-up">
            <p>
              Hi ! I’m Nemo Fazakerley, a junior digital designer based in Paris. 
            </p>
          </div>
          <div class="footer-container-about-txt-down">
            <p>
              I am actively looking for a 5 months internship in Berlin, Warsaw or Budapest.  Feel free to contact me !
            </p>
          </div>
        </div>
      </div>
      <div class="footer-container-connect">
        <div class="footer-container-connect-title">
          Let's connect
        </div>
        <div class="footer-container-connect-list">
          <ul class="footer-container-connect-list-up">
            <li><a href="mailto:#">Mail</a></li>
            <li><a href="https://dribbble.com/azckaldi" target="_blank">Dribbble</a></li>
            <li><a href="https://www.malt.fr/profile/nemofazakerley" target="_blank">Malt</a></li>
          </ul>
          <ul class="footer-container-connect-list-down">
            <li><a href="https://www.linkedin.com/in/nemofazakerley/" target="_blank">LinkedIn</a></li>
            <li><a href="https://www.behance.net/nemofazakerley" target="_blank">Behance</a></li>
            <!-- <li><a href="" target="_blank"></a></li> -->
          </ul>
        </div>
      </div>
      <div class="footer-container-resume">
        <div class="footer-container-resume-title">
          Resume
        </div>
        <div class="footer-container-resume-txt">
          You can download my resume here : <a href="#" download="resume.pdf">nemofazakerley.pdf</a>
        </div>
      </div>
      <div class="footer-container-credits">
        2019 - Nemo Fazakerley
      </div>
    </div>
  </footer>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>

footer{
  width: 80%;
  margin: 3rem auto;
  margin-bottom: 0;

  .footer-container{
    &-about{
      display: flex;
      justify-content: space-between;
      margin-top: 8rem;

      &-title{
        font-size: 4rem;
        font-weight: 600;
      }
      &-txt{
        width: 38%;
        margin: 3rem;

        &-up{
          font-weight: 200;
          padding: 1.5625rem 0 3rem 0;
          border-top: solid thin;
        }

        &-down{
          font-weight: 600;
        }
      }
    }

    &-connect{
      margin: 6rem 0;
      display: flex;
      justify-content: space-between;

      &-title{
        width: 50%;
        font-size: 4rem;
        font-weight: 600;
      }

      &-list{
        width: 38%;
        border-top: solid thin;
        // padding-top: 3rem;
        margin: 3rem;

        &-up{
          display: flex;
          justify-content: space-between;
          padding: 1.5625rem 0px;

          a{
            text-decoration: none;
            color: white;
          }
        }

        &-down{
          display: flex;
          justify-content: space-between;
          padding: 2rem 0px;

          a{
            text-decoration: none;
            color: white;
          }
        }
      }
    }

    &-resume{
      margin: 6rem 0;
      display: flex;
      justify-content: space-between;

      &-title{
        font-size: 4rem;
        font-weight: 600;
      }
      &-txt{
        font-weight: 200;
        width: 38%;
        border-top: solid thin;
        margin: 3rem;
        padding-top: 1.5625rem;

        a{
          text-decoration: none;
          color: white;
          font-weight: 600;
        }
      }
    } 
    &-credits{
      font-weight: 200;
      border-top: solid thin;
      padding: 2rem 0 5rem 0;
    }
  }
}
</style>