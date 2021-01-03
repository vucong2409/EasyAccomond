<template>
<div class="h-100 p-3 mx-auto">
  <section class="h-100 p-3 mx-auto">
    <div class="cover-container d-flex h-100 p-3 mx-auto flex-column">
      <header class="masthead mb-auto w-100"> 
        <NavBar /> 
      </header>
      <main class="px-3">
        <h1><b>Easy Accomond</b></h1>
        <p class="text-gray"> The<b class="text-white"> #1 </b>house rental app in Vietnam </p>
      </main>

      <footer class="mt-auto">
        <p> Created by <a href="https://twitter.com/vucong24092001" class="text-white"> @vucong2409 </a> </p>
      </footer>
    </div>
  </section>
</div>
</template>

<script>
// @ is an alias to /src
import NavBar from "../components/NavBar"
export default {
  name: 'Home',
  components: {
    NavBar
  }
}
</script>

<style scoped>
  section {
    height: 100vh;
    scroll-snap-align: start;
  }

  footer {
    color : gray
  }
  
  .cover-container {
    max-width: 42em;
  }

  main {
    font-size: 40px;
  }

  .text-gray {
    color: gray;
  }

</style>