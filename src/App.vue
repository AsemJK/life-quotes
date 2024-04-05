<script setup>
import HelloWorld from "./components/HelloWorld.vue";
</script>

<template>
  <div>
    <a href="https://asemalsaiyadi.onrender.com" target="_blank">
      <img src="/src/assets/logo-dark.png" class="logo" alt="Vite logo" />
    </a>
  </div>
  <HelloWorld msg="Islamic Quotes" />
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
