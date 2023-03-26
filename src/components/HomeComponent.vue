<script setup>
import { ref } from "vue";
import ParticlesBackground from "./ParticlesBackground.vue";

const count = ref(0);
</script>

<template>
  <div id="home">
    <ParticlesBackground></ParticlesBackground>
    <div class="greeting">
      <h2>Hello!</h2>
      <h2>My name is <span class="handwriting"> Alexander Evsikov</span></h2>
      <h2>And I am a <span class="handwriting"> Software Developer</span></h2>
    </div>
    <div class="mobile">
      <h2>Hello! My name is</h2>
      <h2><span class="handwriting"> Alexander Evsikov</span></h2>
      <div class="delimiter"></div>
      <h2>I am a professional</h2>

      <h2><span class="handwriting"> Software Developer</span></h2>
    </div>
    <div class="space"></div>
    <div class="space"></div>
    <div class="space"></div>
    <div class="socials">
      <h2>Download Resume</h2>
      <div class="resume_buttons">
        <a href="../../Resume-Alexander-Evsikov-ru.pdf">
          <h2>
            <img src="../assets/download-svgrepo-com.svg" alt="" />
            RU
          </h2>
        </a>
        <a href="../../Resume-Alexander-Evsikov-en.pdf">
          <h2>
            <img src="../assets/download-svgrepo-com.svg" alt="" />
            EN
          </h2>
        </a>
      </div>
    </div>
    <div class="space"></div>
    <div class="space"></div>
    <div class="space"></div>
  </div>
</template>

<style scoped lang="scss">
#home {
  min-height: calc(100vh - 4em);
  display: flex;
  flex-direction: column;
  justify-content: center;
  gap: 0;
  width: 100vw !important;
  overflow: hidden;
  /* border:1px solid #fafafa; */

  .greeting,
  .mobile {
    display: flex;
    margin: 0 auto;
    flex-direction: column;
    color: var(--text);
  }
  .mobile {
    text-align: center;
  }

  h2 {
    font-family: "MsMadi";
    font-size: 2.5em;
    margin: 0;
    word-spacing: 0.3em;
    .handwriting {
      font-size: 1.5em;
      color: var(--accent);
    }
  }

  .socials {
    display: flex;
    justify-content: center;
    color: var(--text);
    align-items: center;
    gap: 1em;
    font-family: "MsMadi", "HachiMaru";

    .resume_buttons {
      display: flex;
      gap: 1em;
    }

    a {
      color: var(--text);
      h2 {
        font-family: "MsMadi", "HachiMaru";
        font-size: 2.2em;
        display: flex;
        align-items: center;
        gap: 0.3em;
        background: #0007;
        padding: 0.1em 0.4em;
        border-radius: 10px;
        transition: all 0.2s ease;
        img {
          height: 1em;
        }
        &:hover {
          background: #000b;
          transform: scale(1.02);
        }
      }
      &:hover {
        color: var(--accent);
      }
    }
  }
}

/* Min-width: 320px (smaller phone viewpoints) */
@media only screen and (max-width: 320px) {
  #home {
    .mobile {
      display: flex;
    }
    .greeting {
      display: none;
    }
    h2 {
      font-size: 1em;
    }
    .socials {
      display: flex;
      flex-direction: column;
    }
  }
}
/* Min-width: 320px (smaller phone viewpoints) */
@media only screen and (min-width: 320px) {
  #home {
    .mobile {
      display: flex;
    }
    .greeting {
      display: none;
    }
    h2 {
      font-size: 2em;
    }
    .socials {
      display: flex;
      flex-direction: column;
    }
  }
}

/* Min-width: 480px (small devices and most phones) */
@media only screen and (min-width: 480px) {
  #home {
    .mobile {
      display: flex;
    }
    .greeting {
      display: none;
    }
    h2 {
      font-size: 2em;
    }
  }
}

/* Min-width: 768px (most tablets) */
@media only screen and (min-width: 768px) {
  #home {
    .mobile {
      display: none;
    }
    .greeting {
      display: flex;
    }
    h2 {
      font-size: 2em;
    }
  }
}

/* Min-width: 992px (smaller desktop viewpoints) */
@media only screen and (min-width: 992px) {
  #home {
    h2 {
      font-size: 2.5em;
    }
  }
}
</style>
