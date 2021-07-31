<template>
  <p>Loop example</p>
  <ul>
    <li v-for="item in items" v-bind:key="item.id">{{ item.title }}</li>
  </ul>

  <p>s</p>
  <consume-test />
  <p>e</p>
</template>

<script>
import ConsumeTest from './ConsumeTest.vue'

export default {
  data() {
    return {
      items: [{ id: 1, title: 'Item 1' }, { id: 2, title: 'Item 2' }]
    }
  },
  components: {
    ConsumeTest
  }
}
</script>