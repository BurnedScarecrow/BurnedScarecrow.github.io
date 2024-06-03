<script setup>
import { ref } from "vue";

const props = defineProps({
  language: {
    type: String,
    required: true,
  },
});
</script>

<template>
  <section id="experience" class="container">
    <svg class="wave" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320">
      <path
        fill="#fafafa"
        fill-opacity="1"
        d="M0,96L120,85.3C240,75,480,53,720,42.7C960,32,1200,32,1320,32L1440,32L1440,0L1320,0C1200,0,960,0,720,0C480,0,240,0,120,0L0,0Z"
      ></path>
    </svg>
    <h2 class="section-header">
      Experience
      <!-- <span class="lang" @click="lang = lang == 'ru' ? 'en' : 'ru'">{{ lang == "ru" ? "en" : "ru" }}</span> -->
    </h2>

    <div class="experience_content">
      <div class="work-title">
        <h2>Frontend Developer</h2>
        <h3>Freelance</h3>
        <h3>2018</h3>
      </div>
      <div class="work-info">
        <p>
          <i>Responsibilities:</i>
          Developing a web pages using Vue JS. Fixing bugs of the layout.
          Connecting frontend to backend using REST API. Use the concept of a
          SPA to implement a selling service. Deploy web-sites to AWS.
        </p>
        <p>
          <i>Used skills:</i> HTML · CSS · SASS · Figma · Single Page
          Applications · Amazon Web Services (AWS) · Nginx · VueJS · Linux ·
          Bash
        </p>
      </div>

      <!-- --------------------------- -->

      <div class="work-title">
        <h2>Fllstack Developer</h2>
        <h3>Freelance</h3>
        <h3>2019</h3>
      </div>
      <div class="work-info">
        <p>
          <i>Responsibilities:</i> Developing a web application on the Mongo
          Express Vue Node stack. Creation of a server-side CRUD application.
          Implement SPA for selling services. Using AWS and Docker to Deploy a
          Microservice Application.
        </p>
        <p>
          <i>Used skills:</i> Express.js · Django · HTML · CSS · SASS · Docker ·
          Figma · SPA · AWS · Nginx · VueJS · NuxtJS · NodeJS · Python ·
          TypeScript · NestJS · JavaScript · Linux · Bash
        </p>
      </div>
      <!-- --------------------------- -->

      <div class="work-title">
        <h2>Data Engineer</h2>
        <h3>St. Petersburg ETU "LETI"</h3>
        <h3>2020</h3>
      </div>
      <div class="work-info">
        <p>
          <i>Responsibilities:</i> Create datasets from logs raw data. Modify
          datasets by adding new metrics. Creating models for Mashine Learning
          (ML). Implement predictive models. Use Markov's model for user actions
          prediction in the application.
        </p>
        <p>
          <i>Used skills:</i> ExpressJS · Django · ML · Python · Pandas ·
          Catboost · SciKit Learn · Math Statistics · Scientific research
        </p>
      </div>

      <!-- --------------------------- -->

      <div class="work-title">
        <h2>Web Developer</h2>
        <h3>ProCSy</h3>
        <h3>March 2022</h3>
      </div>
      <div class="work-info">
        <p>
          <i>Responsibilities: </i> Design and development of a fintech web
          application. Testing.
        </p>
        <p>
          <i>Used skills:</i> Javascript · TypeScript · Jest · NestJS · NuxtJS ·
          VueJS · Vuex · Axios · Figma
        </p>
      </div>

      <!-- --------------------------- -->

      <div class="work-title">
        <h2>QA Engineer</h2>
        <h3>ProCSy</h3>
        <h3>June 2022</h3>
      </div>
      <div class="work-info">
        <p>
          <i>Responsibilities:</i> Testing high performance crypto-network for
          transactions. Write E2E tests and integration tests.
        </p>
        <p>
          <i>Used skills:</i> JavaScript · Jest · E2E Tests · Integration tests
        </p>
      </div>

      <!-- --------------------------- -->

      <div class="work-title">
        <h2>Backend Engineer</h2>
        <h3>Comfortel</h3>
        <h3>September 2022</h3>
      </div>
      <div class="work-info">
        <p>
          <i>Responsibilities:</i> Backend engineer with speciality in restfull
          APIs, network security and backend development. Implementing and
          testing server side part of smart home and IoT management application.
          Implementing microservice architecture with Nest.js, Kafka, HTTP and
          MQTT.
        </p>
        <p>
          <i>Used skills:</i> IoT · Smart Home · Jenkins · NodeJS · Python ·
          Apache Kafka · TypeScript · Jest · MongoDB · Open API · Microservices
          · MQTT · NestJS · Network Security
        </p>
      </div>

      <!-- --------------------------- -->

      <div class="work-title">
        <h2>Leed Backend Developer</h2>
        <h3>T. Hunter</h3>
        <h3>June 2023</h3>
      </div>
      <div class="work-info">
        <p v-show="props.language == 'en'">
          <i>Responsibilities:</i> Overseeing the design, development, and
          maintenance of the server-side logic, databases, and APIs of web
          applications. I also provided technical guidance, mentorship to the
          backend development team, and ensured the scalability, performance,
          and security of the backend systems.
        </p>
        <p v-show="props.language == 'ru'">
          <i>Обязанности:</i> Контроль за проектированием, разработкой и
          поддержкой серверной логики, баз данных и API веб-приложений. Также я
          предоставлял техническое руководство, наставничество команде
          разработчиков и обеспечивал масштабируемость, производительность и
          безопасность серверной части.
        </p>
        <p>
          <i>Used skills:</i> TypeScript · OSINT · NestJS · Python · RabbitMQ ·
          PostgrSQL · Docker · Open API · Microservices · Golang · Alhorithms ·
          Information Security · Leadership · GitLab
        </p>
      </div>
    </div>
  </section>
  <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320">
    <path
      fill="#fafafa"
      fill-opacity="1"
      d="M0,192L120,202.7C240,213,480,235,720,250.7C960,267,1200,277,1320,282.7L1440,288L1440,320L1320,320C1200,320,960,320,720,320C480,320,240,320,120,320L0,320Z"
    ></path>
  </svg>
</template>

<style scoped lang="scss">
#experience {
  position: relative;
  display: flex;
  flex-direction: column;
  width: 100vw;
  color: var(--text);
  padding: 100px 0;

  .section-header {
    margin-bottom: 50px;
  }

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

  .experience_content {
    display: grid;
    grid-template-columns: 2fr 3fr;
    gap: 50px;
    .work-title {
      display: flex;
      flex-direction: column;
      justify-content: start;
      align-items: end;
      // height: 200px;
      // margin: 10px 0;

      h2 {
        color: var(--accent);
        font: 1.5em "Jost";
      }
      h3 {
        font: 1.3em "Jura";
      }
    }
  }

  .work-info {
    display: flex;
    flex-direction: column;
    justify-content: start;
    box-sizing: border-box;
    p {
      margin-bottom: 10px;
      padding-right: 100px;
    }
  }
}

/* Min-width: 320px (smaller phone viewpoints) */
@media only screen and (max-width: 320px) {
  #experience {
    .experience_content {
      display: flex;
      flex-direction: column;
      gap: 20px;
      .work-title {
        align-items: start;
      }
    }

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
@media only screen and (max-width: 1200px) {
  #experience {
    .experience_content {
      display: flex;
      flex-direction: column;
      width: 90%;
      margin: 0 auto;
      gap: 20px;

      .work-title {
        align-items: start;
        width: 100%;
        padding: 0.5em 2em;
      }
    }

    h2 {
      font-size: 1.5em;
    }
    p {
      width: 100%;
      font-size: 1em;
    }

    .work-info {
      width: 100%;
      padding: 0 2em;
      p {
        text-align: justify;
        color: var(--text);
        padding: 0;
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
    .work-title {
      align-items: start;
    }

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

    .work-title {
      font-size: 1.3em;
      align-items: start;
    }
  }
}
</style>
