<template>
  <provide-test>
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    <TestClick />
    <p>Second line {{ hello }}</p>
    <sub-test>
      <test-loop />
      <test-form />
    </sub-test>
  </provide-test>
</template>

<script>
import * as Vue from 'vue'
import TestClick from './components/TestClick.vue'
import HelloWorld from './components/HelloWorld.vue'
import TestLoop from './components/TestLoop.vue'
import TestForm from './components/TestForm.vue'
import SubTest from './components/SubTest.vue'
import ProvideTest from './components/ProvideTest.vue'

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
    TestForm,
    SubTest,
    ProvideTest
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
