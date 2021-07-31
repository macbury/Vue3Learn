<template>
  <input v-model="item.title" placeholder="Edit me!" />
</template>

<script>
export default {
  data() {
    return {
      item: {
        title: 'Hello'
      }
    }
  }
}
</script>