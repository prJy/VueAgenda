<template>
<div class="container">
  <div id="app">
    <MainPageMenu />
    <router-view/>
  </div>
</div>
</template>

<script>
import MainPageMenu from './components/MainPageMenu';

export default {
  name: 'App',
  data() {
    return {
      usuario: {
        nome: 'anderson',
      },
    };
  },
  components: {
    MainPageMenu,
  },
};
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
