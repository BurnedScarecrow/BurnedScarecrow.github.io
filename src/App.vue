<script setup>
import AboutComponent from "./components/AboutComponent.vue";
import HomeComponent from "./components/HomeComponent.vue";
import TopLine from "./components/TopLine.vue";
</script>

<template>
  <div id="app">
    <TopLine></TopLine>
    <HomeComponent></HomeComponent>
    <AboutComponent></AboutComponent>
    <!-- <HelloWorld msg="Vite + Vue" />
      <HelloWorld msg="Vite + Vue" />
      <HelloWorld msg="Vite + Vue" />
      <HelloWorld msg="Vite + Vue" />
      <HelloWorld msg="Vite + Vue" /> -->
  </div>
</template>

<style scoped>
#app {
  display: flex;
  width: 100vw;
  flex-direction: column;
  overflow-x: hidden;
}
</style>
