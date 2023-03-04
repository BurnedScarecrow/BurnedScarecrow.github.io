<script setup>
import { ref } from 'vue'
import ParticlesBackground from './ParticlesBackground.vue';

const count = ref(0)
</script>

<template>
  <div id="home">
    <ParticlesBackground></ParticlesBackground>
    <div class="greeting">
      <h2>
        Hello!
      </h2>  
      <h2>My name is <span class="handwriting"> Alexander Evsikov</span></h2>
      <h2>
        And I am a <span class="handwriting"> Software Developer</span>
      </h2>
    </div>
    <div class="space"></div>
    <div class="space"></div>
    <div class="space"></div>
  </div> 
</template>

<style scoped lang="scss">
#home{
  min-height: calc(100vh - 4em);
  display: flex;
  flex-direction: column;
  justify-content: center;
  gap: 0;
  /* border:1px solid #fafafa; */
  
  h2 {
    font-family: 'MsMadi';
    font-size: 2.5em;
    margin: 0;
    word-spacing: 0.3em;
    .handwriting{
      font-size: 1.5em;
      color: var(--accent);
    }
  }
}

/* Min-width: 320px (smaller phone viewpoints) */
@media only screen and (max-width: 320px) {
  #home{ h2{
    font-size: 0.8em;
  }}
}
/* Min-width: 320px (smaller phone viewpoints) */
@media only screen and (min-width: 320px) {
  #home{ h2{
    font-size: 1em;
  }}
}

/* Min-width: 480px (small devices and most phones) */
@media only screen and (min-width: 480px) {
  #home{ h2{
    font-size: 1.5em;
  }}
}

/* Min-width: 768px (most tablets) */
@media only screen and (min-width: 768px) {
  #home{ h2{
    font-size: 2em;
  }}
}

/* Min-width: 992px (smaller desktop viewpoints) */
@media only screen and (min-width: 992px) {
  #home{ h2{
    font-size: 2.5em;
  }}
}

</style>