<template>
  <div id="app">
    <div id="editor"></div>
  </div>
</template>

<script>
import ace from 'ace-builds'

export default {
  name: 'App',
  components: {
  },
  mounted () {
    console.log(ace)
    ace.edit("editor");
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
