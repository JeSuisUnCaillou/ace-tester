<template>
  <div id="app">
    <div id="editor"></div>
  </div>
</template>

<script>
import ace from 'ace-builds'

export default {
  name: 'App',
  data () {
    return {
      editor: null
    }
  },
  mounted () {
    this.editor = ace.edit("editor")
    this.editor.setValue('Lorem ipsum dolor sit amet ⌚, consectetur adipiscing elit.\nSuspendisse rutrum nisi elit, vitae sodales orci ullamcorper nec.\nNullam sed quam vel enim 🤦‍♀ sollicitudin vulputate in vel orci.\nInteger iaculis nec massa vitae fringilla. Proin nec bibendum ante.\nEtiam iaculis risus bibendum sapien laoreet, sit amet blandit tellus fermentum.\nCurabitur bibendum, erat vitae malesuada mattis, nunc mauris pellentesque lorem, sed consequat enim augue vitae elit. Nulla sodales eros purus, et dignissim erat cursus vel.')
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
}
html, body, #app {
  min-height: 100vh;
  margin: 0;
}
#app {
  display: flex;
  align-items: center;
  justify-content: center;
}
#editor {
  width: 500px;
  height: 400px;
}
</style>
