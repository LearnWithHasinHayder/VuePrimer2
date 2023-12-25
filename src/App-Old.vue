<script>
import HelloWorld from './components/HelloWorld.vue';

export default {
  components: {
    helloworld:HelloWorld
  },
  setup(){
    function sayHello(){
        return "Hello World!"
    }
    return {
      sayHello,
      message: 'Hello Vue 3 + Vite!!!'
    }
  }
}
</script>

<template>
  <div>
    <a href="https://vitejs.dev" target="_blank">
      <img src="/vite.svg" class="logo" alt="Vite logo" />
    </a>
    <a href="https://vuejs.org/" target="_blank">
      <img src="./assets/vue.svg" class="logo vue" alt="Vue logo" />
    </a>
  </div>

  <h1>{{ message }}</h1>

  <h2> {{ sayHello() }}</h2>

  <helloworld></helloworld>

</template>

<style>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
