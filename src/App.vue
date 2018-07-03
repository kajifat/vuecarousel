<template>
  <div id="app">
    <Navbar></Navbar>
    <div class=container>
      <slick
        ref="slick"
        :options="slickOptions"
      >
        <div v-for="(img, key) in images" :key="key">
          <a :href="img.link"><img :src="img.src" alt=""></a>
        </div>
      </slick>
    </div>
    <div class="test-header"></div>
  </div>
</template>

<script>
import Navbar from './components/Navbar'
import Slick from 'vue-slick'

export default {
  name: "app",
  components: {Navbar, Slick},
  data() {
    return {
      images: [
        {
          link: "http://placehold.it/300x100",
          src: "http://placehold.it/300x100"
        },
        {
          link: "http://placehold.it/300x100",
          src: "http://placehold.it/300x100"
        },
        {
          link: "http://placehold.it/300x100",
          src: "http://placehold.it/300x100"
        },
        {
          link: "http://placehold.it/300x100",
          src: "http://placehold.it/300x100"
        },
        {
          link: "http://placehold.it/300x100",
          src: "http://placehold.it/300x100"
        },
        {
          link: "http://placehold.it/300x100",
          src: "http://placehold.it/300x100"
        },
        {
          link: "http://placehold.it/300x100",
          src: "http://placehold.it/300x100"
        }
      ],
      slickOptions: {
        arrows: false,
        slidesToShow: 3,
        responsive: [
          {
            breakpoint: 600,
            settings: {
              slidesToShow: 1
            }
          }
        ]
      }
    }
  }
}
</script>

<style>
@import '../node_modules/slick-carousel/slick/slick.css';

#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  display: flex;
  justify-content: center;
}

.container {
  padding-top: 70px;
  max-width: 920px;
}

.test-header {
  height: 1000px;
}
</style>
