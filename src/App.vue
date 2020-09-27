<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <funny-jokes></funny-jokes>
    <joke-button></joke-button>
    
  </div>
</template>

<script>
import NormalJoke from './components/normal-joke.vue'
import SnakeJoke from './components/snake-joke.vue'
import LoudJoke from './components/loud-joke.vue'
import JokeButton from './components/joke-button.vue'

export default {
  name: 'App',
  components: {
 
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
