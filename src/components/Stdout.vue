<template>
  <component :is="component" />
</template>

<script>
export default {
  props: {
    component: {
      default: () => ({
        render (h) {
          h('span')
        }
      })
    }
  }
}
</script>

<style lang="scss">
  @import "../scss/mixins";
</style>
