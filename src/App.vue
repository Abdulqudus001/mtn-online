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
@import url('https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/css/bootstrap.min.css');

@font-face {
  font-family: "MTN-sans";
  src: url(./assets/fonts/MTNBrighterSans-Light.ttf);
  font-weight: 100;
}

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

body {
  overflow-x: hidden;
}

#app {
  font-family: MTN-sans, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}

.my-container {
  width: 1200px;
  max-width: calc(100% - 20px);
  margin: 0 auto;
  padding: 0 20px;
}

ul {
  list-style-type: none;
  padding-left: 0;
}
</style>
