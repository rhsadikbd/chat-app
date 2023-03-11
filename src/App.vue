<template>
  <chat-app />
</template>

<script>
import Chat from './components/Chat.vue'

export default {
  name: 'App',
  components: {
    'chat-app': Chat
  }
}
</script>

<style>
  body{
    background: #6c5ce7;
    height: 98vh;
    font-family: sans-serif;
  }
</style>
