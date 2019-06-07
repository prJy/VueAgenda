<template>
  <div id="app">
    <ul class="menu">
      <li><a href=""></a><a href="#/">Inicio</a></li>
      <li><a href=""></a><a href="#/login">Login</a></li>
      <p>{{usuario.nome}}</p>
    </ul>
    <router-view/>
  </div>
</template>

<script>
export default {
  name: 'App',
  data() {
    return {
      usuario: {
        nome: 'anderson',
      },
    };
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
