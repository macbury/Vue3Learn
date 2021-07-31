<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Your Vue.js App"/>
  <TestClick />
  <p>Second line {{ hello }}</p>
  <test-loop />
  <test-form />
</template>

<script>
import * as Vue from 'vue'
import TestClick from './components/TestClick.vue'
import HelloWorld from './components/HelloWorld.vue'
import TestLoop from './components/TestLoop.vue'
import TestForm from './components/TestForm.vue'

export default {
  name: 'App',
  data: function() {
    return {
      hello: Vue.version
    }
  },
  components: {
    HelloWorld,
    TestClick,
    TestLoop,
    TestForm
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
