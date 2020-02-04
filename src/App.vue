<template>
  <div id="app">
    <Header/>
    <Intro/>
    <Body/>
    <Footer/>
  </div>
</template>

<script>
import Header from './components/Header'
import Footer from './components/Footer'
import Intro from './components/Intro'

import Body from './view/Body'

export default {
  name: 'app',
  components: {
    Header,
    Footer,
    Intro,
    Body,
  }
}
</script>

<style>
@import 'assets/css/reset.css';
@import url('https://rsms.me/inter/inter.css');


html { font-family: 'Inter', sans-serif; }


#app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: white;
  background-color: #222222;
}
</style>
