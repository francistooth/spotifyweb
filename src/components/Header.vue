<template>
  <header class="w-full p-4 bg-black flex justify-evenly">  
    <a>Spotify</a>
    <a> searchbar </a>
    <div class="actions flex gap-10">
      <a> sign up </a>
      <a> login </a>
    </div>
  </header>
</template>

<script>
  export default {
    name: "Header",
  };
</script>

<style>
  header {
    position: fixed;
    top: 0;
  }
</style>