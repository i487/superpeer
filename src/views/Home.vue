<template>
  <div class="home">
    <img src="../assets/back-img.png" alt="" class="home__img">
   <Header />
   <div class="container">
     <Intro />
   </div>
   <main class="main">
     <Series />
     <div class="container">
       <Features />
     </div>
   </main>
   <Superpeer-for-you />
   <Carousel />
   <Introducing />
   <Bottom />
   <div class="container">
     <Footer />
   </div>

  </div>
</template>

<script>
import Footer from '../components/Footer.vue';
import Bottom from '../components/Bottom.vue';
import Carousel from '../components/Carousel.vue';
import Features from '../components/Features.vue';
import Header from '../components/Header.vue';
import Intro from '../components/Intro.vue';
import Introducing from '../components/Introducing.vue';
import Series from '../components/Series.vue';
import SuperpeerForYou from '../components/SuperpeerForYou.vue';
// @ is an alias to /src

export default {
  components: { Header, Intro, Series, Features, SuperpeerForYou, Carousel, Introducing, Bottom, Footer },
  name: "Home",
 
};
</script>

<style lang="scss">
.home {
  overflow: hidden;
  position: relative;
  
  &__img {
    width: 100%;
    position: absolute;
    z-index: -1;
    top: 20%;
    animation-name: beat;
    animation-duration: 3s;
    animation-iteration-count: infinite;
  }

  .main {
    background: linear-gradient(180deg, #FFF7E0 0%, #FFFFFF 100%);
  }
}
@keyframes beat {
  0% {
    transform: scale(1);
  }
  50% {
    transform: scale(1.03);
  }
}

@media only screen and (max-width: 750px) {
  .home {
    &__img {
      top: 100px;
    }
  }
}
</style>
