<script setup>
import AboutComponent from "./components/AboutComponent.vue";
import ExperienceComponent from "./components/ExperienceComponent.vue";
import HomeComponent from "./components/HomeComponent.vue";
import SkillsComponent from "./components/SkillsComponent.vue";
import TopLine from "./components/TopLine.vue";
</script>

<template>
  <div id="app">
    <TopLine></TopLine>
    <HomeComponent></HomeComponent>
    <AboutComponent></AboutComponent>
    <SkillsComponent></SkillsComponent>
    <ExperienceComponent></ExperienceComponent>
    <div class="space"></div>
    <div class="space"></div>
    <div class="space"></div>
    <div class="space"></div>
    <div class="space"></div>
    <div class="space"></div>
    <div class="space"></div>
    <div class="space"></div>
    <div class="space"></div>
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
