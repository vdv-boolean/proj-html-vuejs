<script>

  import Header from "./components/Header.vue"
  import Main from "./components/Main.vue"
  import Footer from "./components/Footer.vue"

  export default {
      components: {
        Header,
        Main,
        Footer,
      }
    }

</script>

<template>

  <Header/>
  <Main/>
  <Footer/>

</template>

<style>

  header {
    height: 600px;
    background-image: url(./img/1-hero-image.png);
    background-size: cover;
    background-repeat: no-repeat;
    background-position: center;
  }

  .container {
    width: 1000px;
    height: 100%;
    margin: auto;
  }

</style>
