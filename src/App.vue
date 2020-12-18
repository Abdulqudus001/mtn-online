<template>
  <div id="app">
    <Home />
  </div>
</template>

<script>
import Home from './pages/Home.vue';

export default {
  name: 'App',
  components: {
    Home,
  },
};
</script>

<style lang="scss">
@import url('https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.1/css/all.min.css');
@import url('https://cdnjs.cloudflare.com/ajax/libs/normalize/8.0.1/normalize.min.css');

@font-face {
  font-family: "MTN-sans";
  src: url(./assets/fonts/MTNBrighterSans-Regular.ttf);
}

@font-face {
  font-family: "MTN-sans";
  src: url(./assets/fonts/MTNBrighterSans-Medium.ttf);
  font-weight: 600;
}

@font-face {
  font-family: "MTN-sans";
  src: url(./assets/fonts/MTNBrighterSans-Bold.ttf);
  font-weight: 700;
}

#app {
  font-family: MTN-sans, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}
</style>
