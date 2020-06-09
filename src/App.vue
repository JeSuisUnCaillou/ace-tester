<template>
  <div id="app">
    <pre>
      <textarea>
        Lo🤷‍♂️rem
      </textarea>
    </pre>
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
    this.editor.setValue('Lo🤷‍♂️rem\nip👨‍🎨sum dolor sit amet, consectetur adipiscing elit.\nSus🤦😃📢🔔⌚❌➰⏳pendisse rutrum nisi elit, vitae sodales orci ullamcorper nec.')
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
