<template>
  <div>
    <h2>This is a pop up</h2>
    <button @click="$emit('close')">Close pop up</button>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld', 
  props: {
    msg: String
  },
  emits: ['close'],  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
