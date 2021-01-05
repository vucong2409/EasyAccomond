<template>
<div class="h-100 w-100 mx-auto">
  <section class="h-100 w-100 mx-auto">
    <div class="cover-container d-flex h-100 pb-3 mx-auto flex-column">
      <header class="masthead mb-auto w-100"> 
        <NavBar /> 
      </header>
      <main class="px-3 w-100">
        <h1><b>Easy Accomond</b></h1>
        <p class="text-gray"> The<b class="texj-white"> #1 </b>house rental app in Vietnam  </p>
        <b-icon icon="arrow-down-short" animation="cylon-vertical" font-scale="2" class="mx-5"></b-icon>
      </main>

      <footer class="mt-auto">
        <p> Created by <a href="https://twitter.com/vucong24092001" class="text-white"> @vucong2409 </a> </p>
      </footer>
    </div>
  </section>

  <section class="h-100 py-3 mx-auto second-pane" >
    <div class=" d-flex mx-5 h-100 py-5 mx-auto flex-column plan-container">
      <header class="masthead mb-auto w-100">
        <h3 class="section-header"> Choose your plan </h3>
      </header>

      <main class="px-3 d-flex justify-content-center">
          <div class="container border rounded bg-white mx-5 text-dark p-5 shadow" data-aos="fade-right">
            <h4> Basic </h4>
            <h1> $0 </h1>
            <hr/>
            <p class="content"> Good house quality </p>
            <p class="content"> <b> 1 </b> house at the same time </p>
            <p class="content"> <b> 10% </b> discount in 3 month </p> 
            <b-button squared outline-danger class="bg-dark text-white mt-5" size="lg"> Learn More </b-button>
          </div>
          <div class="container border rounded bg-dark mx-5 text-white p-5 shadow" data-aos="fade-up">
            <h4> Standard </h4>
            <h1> $5 </h1>
            <hr/>
            <p class="content"> Good house quality </p> 
            <p class="content"> <b> 2 </b> house at the same time </p>
            <p class="content"> <b> 20% </b> discount in 3 month </p>
            <b-button squared outline-danger class="bg-white text-dark mt-5" size="lg"> Learn More </b-button>
          </div>
          <div class="container border rounded bg-danger mx-5 text-white p-5 shadow" data-aos="fade-left">
            <h4> Premium </h4>
            <h1> $10 </h1>
            <hr/>
            <p class="content"> Best house quality </p>
            <p class="content"> <b> 3 </b> house at the same time </p>
            <p class="content"> <b> 30% </b> discount in 3 month </p>
            <b-button squared outline-danger class="bg-white text-danger mt-5" size="lg"> Learn More </b-button>
          </div>
      </main>

      <footer class="mt-auto pb-0">
        <small class="pb-0 mb-0"> <i> *VAT included </i> </small>
      </footer>
    </div>
  </section>

  <section class="h-100 p-3 mx-auto">
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
  
  .content {
    font-size: 20px;
  }
  hr {
    width: 75%;
  } 
  .section-header {
    font-size: 40px;
  }
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

  .second-pane {
    background: white;
    color: black;
  }


</style>