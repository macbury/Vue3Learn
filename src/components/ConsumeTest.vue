<template>
  <p>
    Consume Test: {{ this.store.item }}
  </p>
</template>

<script>
export default {
  name: 'ConsumeTest',
  inject: ['store'],
  created() {
    console.log(this.store)
  }
}
</script>