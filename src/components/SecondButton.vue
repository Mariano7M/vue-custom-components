<template>
  <button @click="onClick()">
    {{label}}
  </button>
</template>

<script>
export default {
  name: 'SecondButton',
  props: {
    label: {
      type: String,
      require: true,
      default: 'Second button'
    }
  },
  setup() {
    function onClick() {
      console.log('on click from second button')
    }
    return {onClick}
  }
}
</script>

<style>

</style>