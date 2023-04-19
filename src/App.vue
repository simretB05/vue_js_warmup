<template>
  <div id="app">
<fun-component></fun-component>
  </div>
</template>

<script>
import FunComponent from './components/FunComponent.vue';
export default {
  name: 'App',
  components: {
FunComponent
  }
}
</script>

<style>
*{margin: 0;
padding: 0;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;

}
</style>
