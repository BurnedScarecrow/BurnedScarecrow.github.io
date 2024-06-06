<script setup>
import { computed, ref } from "vue";

const date = ref("date");

date.value = new Date().getFullYear();
</script>

<template>
  <section id="contacts">
    <div class="container">
      <h2 class="section-header">Contact me</h2>
      <hr />
      <div class="space"></div>
      <div class="space"></div>
      <div class="contacts-section">
        <div class="ref">
          <img src="../assets/github-mark.svg" alt="" />
          <a href="https://github.com/BurnedScarecrow" target="_blank">
            BurnedScarecrow
          </a>
        </div>
        <div class="ref">
          <img src="../assets/email.png" alt="" />
          <a href="mailto:evsik.sasha@gmail.com" target="_blank">
            evsik.sasha@gmail.com
          </a>
        </div>
        <div class="ref">
          <img src="../assets/linkedin.png" alt="" />
          <a href="https://www.linkedin.com/in/cawa/" target="_blank"> cawa </a>
        </div>
      </div>
      <div class="space"></div>
      <footer>Alexander Evsikov &copy; {{ date }}</footer>
    </div>
  </section>
</template>

<style scoped lang="scss">
#contacts {
  background: var(--text);
  flex-direction: column;
  justify-content: center;
  width: 100vw;
  color: var(--bg);
  padding-bottom: 50px;
  margin-top: -2px;

  footer {
    text-align: center;
    font-family: "Jura";
  }

  .lang {
    border-color: var(--bg) !important;
    &:hover {
      background: var(--bg) !important;
      color: var(--text) !important;
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

  .contacts-section {
    display: flex;
    gap: 30px;
    flex-wrap: wrap;
    justify-content: center;

    .ref {
      justify-content: center;
      display: flex;
      height: 2em;
      font: 1.5em "Jura";

      img {
        height: 1.5em;
        margin-right: 20px;
      }

      a {
        font-size: 1.2em;
        color: var(--bg);
      }
    }
  }
}

/* Min-width: 320px (smaller phone viewpoints) */
@media only screen and (max-width: 320px) {
  #contacts {
    h2 {
      font-size: 1.2em;
    }

    p {
      width: 100%;
      font-size: 1em;
    }
  }
}
/* Min-width: 320px (smaller phone viewpoints) */
@media only screen and (min-width: 320px) {
  #contacts {
    h2 {
      font-size: 1.5em;
    }
    p {
      width: 100%;
      font-size: 1em;
    }
    .contacts-section {
      .ref {
        font: 1em "Jura";
      }
    }
  }
}

/* Min-width: 480px (small devices and most phones) */
@media only screen and (min-width: 480px) {
  #contacts {
    h2 {
      font-size: 1.5em;
    }
    p {
      width: 100%;
    }
  }
}

/* Min-width: 768px (most tablets) */
@media only screen and (min-width: 768px) {
  #contacts {
    .wave {
      margin-top: -100px;
    }
    h2 {
      font-size: 2em;
    }
  }
}

/* Min-width: 992px (smaller desktop viewpoints) */
@media only screen and (min-width: 992px) {
  #contacts {
    h2 {
      font-size: 2.5em;
    }
    p {
      width: 80%;
    }
    .contacts-section {
      .ref {
        font: 1.5em "Jura";
      }
    }
  }
}
</style>
