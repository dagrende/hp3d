<template>
  <div class="toolbar">
    <div v-on:click="$emit('addCube')">cube</div>
    <div>cylinder</div>
    <div>union</div>
    <div>subtract</div>
    <div>intersection</div>
  </div>
</template>

<script>
export default {
  name: 'buttons',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.toolbar {
  display: flex;
  flex-direction: row;
  padding-left: 3px;
}
.toolbar > div {
  flex: 0;
  padding: 2px;
  margin: 4px 2px 3px 0;
  background-color: #ddd;
}

</style>
