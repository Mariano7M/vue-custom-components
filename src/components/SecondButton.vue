<template>
  <button>
    {{ label }}
  </button>
</template>

<script>
export default {
  name: 'SecondButton',
  props: {
    label: {
      type: String,
      require: true,
      default: 'Second button',
    },
  },
}
</script>
