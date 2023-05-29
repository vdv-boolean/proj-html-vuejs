<script>
import Navbar from "./Navbar.vue"
import Jumbo from "./Jumbo.vue"

  export default {
      components: {
        Navbar,
        Jumbo,
      }
    }
</script>

<template>

    <header>
        <div class="container">
            <Navbar/>
            <Jumbo/>
        </div>
    </header>
    
</template>

<style scoped>
    .container {
        color: white;
    }

</style>
