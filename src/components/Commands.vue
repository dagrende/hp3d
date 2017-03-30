<template>
  <div class="cmdlist">
    <div v-for="cmd in cmds">
      <command name="cmd"></command>
    </div>
  </div>
</template>

<script>
import Command from './Command'

export default {
  props: ['cmds'],
  name: 'commands',
  components: {
    Command
  },
  data () {
    return {
      commands: ['cmd1', 'cmd2', 'cmd3']
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.cmdlist {
  flex: 1;
  overflow: scroll;
  border-bottom: 1px solid green;
}
</style>
