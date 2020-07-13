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
    this.editor.setValue('je⛵suis👯‍♀uncaillou\nho🏴󠁧󠁢󠁥󠁮󠁧󠁿la\nbonj🕵️‍♂️our je m\'appelle Jordy\nLo🤷‍♂️rem\nip👨‍🎨sum dol’or sit amet, consectetur adipiscing elit.\nSus🤦😃📢🔔⌚❌➰⏳pendisse rutrum nisi elit')
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
  width: 100%;
  height: 400px;
  font-size: 3rem;
}
</style>
