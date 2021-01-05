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
        <p> Created by <a href= "https://twitter.com/vucong24092001" class="text-white"> @vucong2409 </a> </p>
      </footer>
    </div>
  </section>

  <section class="h-100 py-3 mx-auto second-pane" >
    <div class="d-flex mx-5 h-100 py-5 mx-auto flex-column">
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

  <section class="h-100 py-3 mx-auto third-pane">
    <div class="d-flex px-5 h-100 py-5 mx-auto flex-column plan-container">
      <header class="masthead mb-auto w-100">
      </header>

      <main class="px-3 d-flex justify-content-center">
      </main>

      <footer class="mt-auto">
      </footer>
    </div>
  </section>

  <section class="py-3 mx-auto sponsor bg-white text-dark">
    <header class="w-100 mb-auto">
      <h1> Our Partner </h1>
    </header>
  </section>

  <section class="py-3 mx-auto footer text-white">
    <main class="footer d-flex my-5 px-3 justify-content-center">
      <div class="container text-left px-5"> 
        <h5> EzyAccomond </h5>
        <p class="footer-text pb-3"> Lorem ipsum dolor sit amet, consectetur adipisicing elit. Cum incidunt architecto soluta laboriosam, perspiciatis, aspernatur officiis esse. </p>
        <p class="footer-text pb-3 contact"> <b-icon-facebook class="mr-2 contact mx-1"> </b-icon-facebook> facebook.com/ezacommond </p>
        <p class="footer-text pb-3 contact"> <b-icon-twitter class="mr-2 contact mx-1"> </b-icon-twitter> twitter.com/ezacommond </p>
      </div>
      
      <div class="container text-left px-5">
        <h5> Navigation </h5>
      </div>

      <div class="container text-left px-5">
        <h5> Top house monthly </h5>
      </div>

      <div class="container text-left px-5">
        <h5> Newletters </h5>
        <p class="footer-text pb-2"> Sign Up for Our Newsletter to get Latest Updates and Offers. <br/> Subscribe to receive news in your inbox. </p> 
        <input type="email" squared class="p-1 bg-dark text-white newletter" placeholder="Enter your email" />
        <b-button squared class="newletter-button text-white mt-3">SUBSCRIBE</b-button>
      </div>

    </main>
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
  .newletter-button {
    background-color: royalblue;
    width: 93%;
  }
  .newletter {
    font-size: 20px;
    border-radius: 0 !important;
    border-color: white;
    border-width: 0;
    width: 93%;
  }
  h5::after {
    display: block;
    height: 4px;
    background-color: #274abb;
    width: 50px;
    content: "";
    margin-top: 0.7rem;
    margin-bottom: 1.5rem;
  }
  .contact {
    margin-bottom: 0px !important;
  } 
  .footer-text {
    font-size: 16px !important;
  }
  
  .footer {
    height: 31vh !important;
    background: #232733;
    font-size: 20px;
  }

  .sponsor {
    height: 30vh !important;
  }
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