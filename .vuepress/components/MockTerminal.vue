<template lang="pug">
  .terminal-root
    .terminal-titlebar
      .window-controls
        .button.close
        .button.minimize
        .button.maximize
    .terminal-container
      .terminal-text
        div
          span $ 
          span.keyword source 
          span.string "TerminalDaily.sh"
        div.keyword
          span $ 
          span.keyword ls
        div
          span
            router-link(to="/") README.md 
          span.green.keyword
            router-link(to="/hello") HELLO.md 
          span TMUX.md
        div
          span $ 
          span.keyword cat 
          span.string "HELLO.md"
        div
          span $ 
          span.keyword ls
        div
          span $ 
          span.keyword echo 
          span.rainbow lol
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  data: () => ({
    words: 'Terminal Daily! ',
  }),
  mounted() {},
})
</script>


<style lang="sass" scoped>
  @import "../styles/mock-terminal.sass"
</style>

