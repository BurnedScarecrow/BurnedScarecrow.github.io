<script setup>
import AboutComponent from "./components/AboutComponent.vue";
import ContactsComponent from "./components/ContactsComponent.vue";
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
    <ContactsComponent></ContactsComponent>
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
