<template>
  <div>
    <button class="mnho-btn" @click="onClick()">{{label}}</button>
  </div>
</template>

<script>
import {ref} from 'vue'

export default {
  name: 'Button',
  setup(_,context) {
    const label = ref('My button')
    function onClick() {
      console.log('onClick')
      context.emit(true)
    } 

    return {label,onClick}
  }
}
</script>

<style >
  .mnho-btn {
    background-color: #5fa791;
    padding: 5px 10px;
    color: white;
  }
</style>>