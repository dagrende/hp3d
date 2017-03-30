<template>
  <div class="model-viewer">
model
  </div>
</template>

<script>
export default {
  name: 'model',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.model-viewer {
  display: flex;
  flex-direction: column;
  height: calc(100%);

  border-bottom: 1px solid green;
  min-height: 50%;
}

</style>
