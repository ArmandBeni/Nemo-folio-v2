<template>
  <header>
    <div class="header">
      <div class="header-logo">
        <img src="../assets/images/logo.svg" alt="Nf logo">
      </div>
      <div class="nav-info">
        <ul>
          <li><a href="#">resume</a></li>
          <li><a href="#">contact</a></li>
          <li><a href="#">about</a></li>
          <li><a href="#">works</a></li>
        </ul>
      </div>
    </div>
  </header>

</template>

<script>
export default {

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>

  .header{
    height: 10rem;
    padding-bottom: 6rem;
    width: 90%;
    margin: auto;
    display: flex;
    align-items: center;
    justify-content: space-between;

    .header-logo{
      img{
        height: 1.9rem;
      }
    }

    .nav-info{
      padding-top: 1rem;

      ul{
        text-align: right;

        li{
          list-style: none;
          padding: 0.325rem;

          a{
            text-decoration: none;
            color: white;
          }
        }
      }
    }
  }


</style>