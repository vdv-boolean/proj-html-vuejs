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
    background-image: url(public/img/1-hero-image.png);
    background-size: cover;
    background-repeat: no-repeat;
    background-position: center;
  }

  section {
    min-height: 200px;
  }

  .container {
    width: 1000px;
    height: 100%;
    margin: auto;
    text-align: center;
  }

h1,
p {
  margin-inline: 30%;
  text-align: center;
}

  button {
      background-color: none;
      background: none;
      border: none;
      border-radius: 20px;
      padding: 0.5rem;
      padding-inline: 1rem;
      color: white;
      text-transform: uppercase;
  }

  .orange-btn {
        background-color: var(--orange); 
    }

    .violet-btn {
        background-color: var(--violet); 
    }

  a {
        text-decoration: none;
        color: white;
    }

    li {
      list-style: none;
    }

  footer {
    height: 200px;
    background-color: white;
  }
</style>
