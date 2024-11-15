<script>
import Header from './components/Header.vue'
import Player from './components/Player.vue';

export default {
  components: {
    Header,
    Player
  }
}
</script>

<template>
  <Header></Header>
  <Content></Content>
  <Player></Player>
</template>

<style scoped>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
</style>