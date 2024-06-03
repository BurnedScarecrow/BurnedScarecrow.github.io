<script setup>
import AboutComponent from "./components/AboutComponent.vue";
import ContactsComponent from "./components/ContactsComponent.vue";
import ExperienceComponent from "./components/ExperienceComponent.vue";
import HomeComponent from "./components/HomeComponent.vue";
import SkillsComponent from "./components/SkillsComponent.vue";
import TopLine from "./components/TopLine.vue";

import { computed, ref } from "vue";

const lang = ref("en");

const toggleLanguage = () => {
  lang.value = lang.value === "ru" ? "en" : "ru";
};

const displayLanguage = computed(() => (lang.value === "ru" ? "en" : "ru"));
</script>

<template>
  <div id="app">
    <TopLine></TopLine>
    <HomeComponent></HomeComponent>
    <h2 align="center" @click="toggleLanguage">{{ displayLanguage }}</h2>
    <AboutComponent
      :language="lang"
      @languageChanged="toggleLanguage"
    ></AboutComponent>
    <SkillsComponent></SkillsComponent>
    <ExperienceComponent :language="lang"></ExperienceComponent>
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
