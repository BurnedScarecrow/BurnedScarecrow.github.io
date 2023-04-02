<script setup>
import { ref } from "vue";
const lang = ref("en");
</script>

<template>
  <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320">
    <path
      fill="#fafafa"
      fill-opacity="1"
      d="M0,64L60,64C120,64,240,64,360,74.7C480,85,600,107,720,144C840,181,960,235,1080,245.3C1200,256,1320,224,1380,208L1440,192L1440,0L1380,0C1320,0,1200,0,1080,0C960,0,840,0,720,0C600,0,480,0,360,0C240,0,120,0,60,0L0,0Z"
    ></path>
  </svg>
  <section id="experience">
    <div class="container">
      <h2 class="section-header">
        <!-- Experience -->
        <!-- <span class="lang" @click="lang = lang == 'ru' ? 'en' : 'ru'">{{ lang == "ru" ? "en" : "ru" }}</span> -->
      </h2>
    </div>
  </section>
</template>

<style scoped lang="scss">
#experience {
  margin-top: -20px;
  flex-direction: column;
  justify-content: center;
  width: 100vw;
  color: var(--text);
  padding-bottom: 100px;

  .lang {
    border-color: var(--text) !important;
    &:hover {
      background: var(--text) !important;
      color: var(--bg) !important;
    }
  }

  p {
    font-family: "Jura";
    text-align: justify;
    font-size: 1.2em;
    border-radius: 0.3em;
    box-sizing: border-box;
    padding: 1em;
    background: rgba(0, 0, 0, 0.5);
    box-shadow: 7px 10px 5px 0px rgba(0, 0, 0, 0.4);
  }

  .experience-section {
    h2 {
      font: 1.7em "Jura";
    }
    .experience-list {
      font-family: "Jost";
      display: flex;
      flex-wrap: wrap;
      width: 100%;
      gap: 1em;
      margin-top: 1em;

      .skill {
        color: var(--bg);
        display: flex;
        align-items: center;
        background: #fff;
        font-size: 1.3em;
        box-shadow: 1px 1px 7px 0 rgba(0, 0, 0, 0.2);
        border-radius: 20px;
        padding: 0 1em;
        height: 40px;
        gap: 0.4em;
        justify-content: center;
        cursor: pointer;
        transition: all 0.2s ease;
        border: 1px solid transparent;
        box-sizing: border-box;
        &:hover {
          transform: scale(1.05);
          border: 1px solid var(--accent);
        }

        img {
          height: 1em;
        }
      }
    }
  }
}

/* Min-width: 320px (smaller phone viewpoints) */
@media only screen and (max-width: 320px) {
  #experience {
    h2 {
      font-size: 1.2em;
    }

    p {
      width: 100%;
      font-size: 1em;
    }
    .experience-section {
      h2 {
        font: 1em "Jura";
      }
      .experience-list {
        font-size: 0.7rem;
      }
    }
  }
}
/* Min-width: 320px (smaller phone viewpoints) */
@media only screen and (min-width: 320px) {
  #experience {
    h2 {
      font-size: 1.5em;
    }
    p {
      width: 100%;
      font-size: 1em;
    }

    .experience-section {
      h2 {
        font: 1.2em "Jura";
      }
      .experience-list {
        font-size: 0.7rem;
      }
    }
  }
}

/* Min-width: 480px (small devices and most phones) */
@media only screen and (min-width: 480px) {
  #experience {
    h2 {
      font-size: 1.5em;
    }
    p {
      width: 100%;
    }

    .experience-section {
      .experience-list {
        font-size: 0.8rem;
      }
    }
  }
}

/* Min-width: 768px (most tablets) */
@media only screen and (min-width: 768px) {
  #experience {
    .wave {
      margin-top: -100px;
    }
    h2 {
      font-size: 2em;
    }
    .experience-section {
      .experience-list {
        font-size: 1rem;
      }
    }
  }
}

/* Min-width: 992px (smaller desktop viewpoints) */
@media only screen and (min-width: 992px) {
  #experience {
    h2 {
      font-size: 2.5em;
    }
    p {
      width: 80%;
    }
  }
}
</style>
