<script setup>
import HelloWorld from "./components/HelloWorld.vue";
</script>

<template>
  <div class="main">
    <a href="https://asemalsaiyadi.onrender.com" target="_blank">
      <img src="/src/assets/logo-dark.png" class="logo" alt="Vite logo" />
      <h3 style="margin: 0">Islamic Quotes</h3>
    </a>
    <HelloWorld />
  </div>
</template>

<style scoped>
.main {
  height: 100%;
  display: grid;
  place-content: center;
  gap: 0em;
  font-family: "Inter", sans-serif;
  text-align: center;
}
.logo {
  height: 5em;
  padding: 0em;
  margin: 0;
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
