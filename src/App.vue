<template>
  <div id="app">
    <navbar/>
    <gallery></gallery>
    <lightbox></lightbox>
    
  </div>
</template>

<script>
import Navbar from './components/Navbar.vue';
import Gallery from './components/Gallery.vue';
import Lightbox from './components/Lightbox.vue';

export default {
  name: 'app',
  components: {
    Gallery,
    Lightbox,
    Navbar
  }
};
</script>

<style>
* {
  box-sizing: border-box;
}

body {
  margin: 0;
  font-family: sans-serif;
}

#app {
  position: relative;
  min-height: 100vh;
  background: #2bc0e4; /* fallback for old browsers */
  background: -webkit-linear-gradient(
    to top,
    #eaecc6,
    #2bc0e4
  ); /* Chrome 10-25, Safari 5.1-6 */
  background: linear-gradient(
    to top,
    #eaecc6,
    #2bc0e4
  ); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */
}

#scroll-end {
  width: 100%;
}
</style>
