<template>
  <slot/>
</template>

<script>
export default {
  provide() {
    return {
      store: {
        item: 1111
      }
    }
  }
}
</script>