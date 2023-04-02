<script setup>
import { ref } from "vue";
const lang = ref("en");
</script>

<template>
  <section id="experience">
    <svg class="wave" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320">
      <path fill="#fafafa" fill-opacity="1" d="M0,192L720,32L1440,160L1440,0L720,0L0,0Z"></path>
    </svg>
    <div class="left">
      <h2 class="section-header">
        Experience
        <span class="lang" @click="lang = lang == 'ru' ? 'en' : 'ru'">{{ lang == "ru" ? "en" : "ru" }}</span>
      </h2>
      <div class="work-title">
        <h2>Frontend Developer</h2>
        <h3>Freelance</h3>
        <h3>2018</h3>
      </div>
      <div class="work-title">
        <h2>Fllstack Developer</h2>
        <h3>Freelance</h3>
        <h3>2019</h3>
      </div>
      <div class="work-title">
        <h2>Data Engineer</h2>
        <h3>St. Petersburg ETU "LETI"</h3>
        <h3>2020</h3>
      </div>
      <div class="work-title">
        <h2>Web Developer</h2>
        <h3>ProCSy</h3>
        <h3>March 2022</h3>
      </div>
      <div class="work-title">
        <h2>QA Engineer</h2>
        <h3>ProCSy</h3>
        <h3>June 2022</h3>
      </div>
      <div class="work-title">
        <h2>Backend Engineer</h2>
        <h3>Comfortel</h3>
        <h3>September 2022</h3>
      </div>
    </div>
    <div class="right">
      <div class="section-header"></div>
      <div class="work-info">
        <p>
          <i>Responsibilities:</i>
          Developing a web pages using Vue JS. Fixing bugs of the layout. Connecting frontend to backend using
          REST API. Use the concept of a SPA to implement a selling service. Deploy web-sites to AWS.
        </p>
        <p>
          <i>Used skills:</i> HTML · CSS · SASS · Figma · Single Page Applications · Amazon Web Services (AWS)
          · Nginx · VueJS · Linux · Bash
        </p>
      </div>
      <div class="work-info">
        <p>
          <i>Responsibilities:</i> Developing a web application on the Mongo Express Vue Node stack. Creation
          of a server-side CRUD application. Implement SPA for selling services. Using AWS and Docker to
          Deploy a Microservice Application.
        </p>
        <p>
          <i>Used skills:</i> Express.js · Django · HTML · CSS · SASS · Docker · Figma · SPA · AWS · Nginx ·
          VueJS · NuxtJS · NodeJS · Python · TypeScript · NestJS · JavaScript · Linux · Bash
        </p>
      </div>
      <div class="work-info">
        <p>
          <i>Responsibilities:</i> Create datasets from logs raw data. Modify datasets by adding new metrics.
          Creating models for Mashine Learning (ML). Implement predictive models. Use Markov's model for user
          actions prediction in the application.
        </p>
        <p>
          <i>Used skills:</i> ExpressJS · Django · ML · Python · Pandas · Catboost · SciKit Learn · Math
          Statistics · Scientific research
        </p>
      </div>
      <div class="work-info">
        <p><i>Responsibilities: </i> Design and development of a fintech web application. Testing.</p>
        <p>
          <i>Used skills:</i> Javascript · TypeScript · Jest · NestJS · NuxtJS · VueJS · Vuex · Axios · Figma
        </p>
      </div>
      <div class="work-info">
        <p>
          <i>Responsibilities:</i> Testing high performance crypto-network for transactions. Write E2E tests
          and integration tests.
        </p>
        <p><i>Used skills:</i> JavaScript · Jest · E2E Tests · Integration tests</p>
      </div>
      <div class="work-info">
        <p>
          <i>Responsibilities:</i> Backend engineer with speciality in restfull APIs, network security and
          backend development. Implementing and testing server side part of smart home and IoT management
          application. Implementing microservice architecture with Nest.js, Kafka, HTTP and MQTT.
        </p>
        <p>
          <i>Used skills:</i> IoT · Smart Home · Jenkins · NodeJS · Python · Apache Kafka · TypeScript · Jest
          · MongoDB · Open API · Microservices · MQTT · NestJS · Network Security
        </p>
      </div>
    </div>
  </section>
</template>

<style scoped lang="scss">
#experience {
  position: relative;
  display: flex;
  width: 100vw;
  color: var(--text);
  .wave {
    position: absolute;
    top: 0;
  }

  .lang {
    border-color: var(--text) !important;
    &:hover {
      background: var(--text) !important;
      color: var(--bg) !important;
    }
  }

  p {
    font-family: "Jost";
    font-size: 1.2em;
    i {
      font-family: "Jura";
    }
  }

  .left,
  .right {
    width: 50%;
    .section-header {
      z-index: 1;
      height: 200px;
    }
  }
  .left {
    display: flex;
    flex-direction: column;
    justify-content: end;
    padding: 200px 100px;
    align-items: end;

    .work-title {
      display: flex;
      flex-direction: column;
      justify-content: start;
      align-items: end;
      height: 200px;
      margin: 10px 0;

      h2 {
        color: var(--accent);
        font: 1.5em "Jost";
      }
      h3 {
        font: 1.3em "Jura";
      }
    }
  }
  .right {
    background: var(--text);
    display: flex;
    flex-direction: column;
    padding: 200px 100px;
    color: var(--bg);

    .work-info {
      display: flex;
      width: 70%;
      flex-direction: column;
      justify-content: start;
      align-items: start;
      height: 200px;
      margin: 10px 0;
      box-sizing: border-box;
      padding: 10px 0;
      p {
        margin-bottom: 10px;
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

    .left,
    .right {
      position: absolute;
      left: 0;
      width: 100%;
      p {
        width: 100%;
      }
    }
  }
}
/* Min-width: 320px (smaller phone viewpoints) */
@media only screen and (max-width: 1200px) {
  #experience {
    h2 {
      font-size: 1.5em;
    }
    p {
      width: 100%;
      font-size: 1em;
    }

    .left,
    .right {
      width: 100%;
      position: absolute;
      background: transparent;
      padding: 0 10%;

      .section-header {
        align-self: start;
      }

      .work-title {
        height: 110px;
        margin-bottom: 340px;
        background: rgba(0, 0, 0, 0.3);
        padding: 0.5em 1em;
        border-radius: 7px;
        backdrop-filter: blur(10px);
      }

      .work-info {
        width: 100%;
        height: 320px;
        margin-top: 130px;
        background: rgba(0, 0, 0, 0.3);
        padding: 1em;
        border-radius: 7px;
        backdrop-filter: blur(10px);
        p {
          text-align: justify;
          color: var(--text);
        }
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
  }
}

/* Min-width: 768px (most tablets) */
@media only screen and (min-width: 768px) {
  #experience {
    h2 {
      font-size: 2em;
    }
  }
}

/* Min-width: 992px (smaller desktop viewpoints) */
@media only screen and (min-width: 992px) {
  #experience {
    h2 {
      font-size: 2.5em;
    }
  }
}
</style>
