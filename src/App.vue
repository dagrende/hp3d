<template>
  <div id="app">
    <model></model>
    <commands v-bind:cmds="this.commands"></commands>
    <buttons v-on:addCube="addCube"></buttons>
  </div>
</template>

<script>
import Model from './components/Model'
import Command from './components/Command'
import Commands from './components/Commands'
import Buttons from './components/Buttons'

export default {
  name: 'app',
  components: {
    Model,
    Commands,
    Command,
    Buttons
  },
  data: function() {return {
    commands: ['cmd1', 'cmd2', 'cmd3', 'cmd4']
  }},
  methods: {
    addCube: function () {
      this.commands.push('another cmd');
    }
  }
}
</script>

<style>
  body, html {
    margin: 0;
    padding: 0;
  }
  #app {
    display: flex;
    flex-direction: column;
    height: calc(100%);
  }
</style>
