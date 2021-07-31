<template>
  <p>Loop example</p>
  <ul>
    <li v-for="item in items" v-bind:key="item.id">{{ item.title }}</li>
  </ul>
</template>

<script>
export default {
  data() {
    return {
      items: [{ id: 1, title: 'Item 1' }, { id: 2, title: 'Item 2' }]
    }
  }
}
</script>