<template>
  <p v-if="showWorks">Works: {{ test }}</p>
  <button v-on:click="sayYes">Yes</button>
  <button v-on:click="sayNo">No</button>
  <button v-on:click="incProp">Triggered</button>
</template>

<script>
export default {
  data() {
    return {
      test: 'works',
      otherProp: 1
    }
  },
  methods: {
    sayYes() {
      this.test = "Yes"
    },
    sayNo() {
      this.test = 'No'
    },
    incProp() {
      this.otherProp += 1
    }
  },
  computed: {
    showWorks() {
      console.log('Triggered')
      return this.test === 'Yes'
    }
  }
}
</script>