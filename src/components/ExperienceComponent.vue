<script setup>

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
    <h2 class="section-header">Experience</h2>

    <div class="experience_content">
      <!-- Lead Backend Developer -->
      <div class="work-title">
        <h2>Lead Backend Developer</h2>
        <h3>T. Hunter</h3>
        <h3>June 2023</h3>
      </div>
      <div class="work-info">
        <p v-show="props.language == 'en'">
          <i>Responsibilities:</i> 
          <ul>
            <li>Design, development, and maintenance of server-side logic, databases, and APIs for web applications.</li>
            <li>Providing technical guidance and mentorship to the backend development team.</li>
            <li>Ensuring scalability, performance, and security of backend systems.</li>
          </ul>
        </p>
        <p v-show="props.language == 'ru'">
          <i>Обязанности:</i> 
          <ul>
            <li>Проектирование, разработка и обслуживание логики серверной части, баз данных и API для веб-приложений.</li>
            <li>Предоставление технического руководства и наставничества команде разработчиков backend.</li>
            <li>Обеспечение масштабируемости, производительности и безопасности серверных систем.</li>
          </ul>
        </p>
        <p>
          <i>Used skills:</i> TypeScript · OSINT · NestJS · Python · RabbitMQ ·
          PostgrSQL · Docker · Open API · Microservices · Golang · Alhorithms ·
          Information Security · Leadership · GitLab
        </p>
      </div>

      <!-- Backend Engineer -->
      <div class="work-title">
        <h2>Backend Engineer</h2>
        <h3>Comfortel</h3>
        <h3>September 2022</h3>
      </div>
      <div class="work-info">
        <p v-show="props.language == 'en'">
          <i>Responsibilities:</i> 
          <ul>
            <li>Designing and implementing RESTful APIs.</li>
            <li>Ensuring network security measures are in place.</li>
            <li>Developing backend systems for smart home and IoT management applications.</li>
            <li>Testing server-side components thoroughly.</li>
            <li>Utilizing microservice architecture with Nest.js, Kafka, HTTP, and MQTT.</li>
          </ul>
        </p>
        <p v-show="props.language == 'ru'">
          <i>Обязанности:</i> 
          <ul>
            <li>Проектирование и реализация RESTful API.</li>
            <li>Обеспечение безопасности сети.</li>
            <li>Разработка серверных систем для управления умным домом и Интернетом вещей.</li>
            <li>Тщательное тестирование серверных компонентов.</li>
            <li>Использование микросервисной архитектуры с помощью Nest.js, Kafka, HTTP и MQTT.</li>
          </ul>
        </p>
        <p>
          <i>Used skills:</i> IoT · Smart Home · Jenkins · NodeJS · Python ·
          Apache Kafka · TypeScript · Jest · MongoDB · Open API · Microservices
          · MQTT · NestJS · Network Security
        </p>
      </div>

      <!-- QA Engineer -->
      <div class="work-title">
        <h2>QA Engineer</h2>
        <h3>ProCSy</h3>
        <h3>June 2022</h3>
      </div>
      <div class="work-info">
        <p v-show="props.language == 'en'">
          <i>Responsibilities:</i> 
          <ul>
            <li>Functional testing of smart contracts and their compliance with stated requirements.</li>
            <li>E2E and integration testing of the blockchain system.</li>
            <li>Security audit, including vulnerability assessment, penetration testing.</li>
            <li>Performance evaluation of the network and its scalability under increasing load or data volume.</li>
          </ul>
        </p>
        <p v-show="props.language == 'ru'">
          <i>Обязанности:</i> 
          <ul>
            <li>Функциональное тестирование работы смарт-контрактов и их соответствия заявленным требованиям.</li>
            <li>E2E и интеграционное тестирование блокчейн системы.</li>
            <li>Аудит безопасности, включая исследование на уязвимости, тестирование на проникновение.</li>
            <li>Оценка производительности сети и ее способности масштабироваться при увеличении нагрузки или объема данных.</li>
          </ul>
        </p>
        <p>
          <i>Used skills:</i> JavaScript · Jest · E2E Tests · Integration tests · Penetration tests · Blockchain
        </p>
      </div>

      <!-- Web Developer -->
      <div class="work-title">
        <h2>Web Developer</h2>
        <h3>ProCSy</h3>
        <h3>March 2022</h3>
      </div>
      <div class="work-info">
        <p v-show="props.language == 'en'">
          <i>Responsibilities: </i> 
          <ul>
            <li>Design and development of web applications for fintech.</li>
            <li>Implementation of frontend functionality </li>
            <li>Integration of backend services and APIs to support currency exchange and cryptocurrency transactions.</li>
            <li>Conducting thorough testing, including unit, integration and E2E testing.</li>
          </ul>
        </p>
        <p v-show="props.language == 'ru'">
          <i>Обязанности:</i> 
          <ul>
            <li>Дизайн и разработка веб-приложения для финтеха.</li>
            <li>Реализация функциональности фронтенда </li>
            <li>Интеграция бэкенд-сервисов и API для поддержки обмена валюты и транзакций с криптовалютой.</li>
            <li>Проведение тщательного тестирования, включая модульное, интеграционное и E2E тестирование.</li>
          </ul>
        </p>
        <p>
          <i>Used skills:</i> Javascript · TypeScript · Jest · NestJS · NuxtJS ·
          VueJS · Vuex · Axios · Figma
        </p>
      </div>

      <!-- Data Engineer -->
      <div class="work-title">
        <h2>Data Engineer</h2>
        <h3>St. Petersburg ETU "LETI"</h3>
        <h3>2020</h3>
      </div>
      <div class="work-info">
        <p v-show="props.language == 'en'">
          <i>Responsibilities:</i> 
          <ul>
            <li>Create datasets from raw mobile app logs.</li>
            <li>Modify datasets by adding new metrics.</li>
            <li>Creating models for Mashine Learning.</li>
            <li>Research and implementation of predictive models.</li>
            <li>Use Markov's model for user actions prediction in the application.</li>
          </ul>
        </p>
        <p v-show="props.language == 'ru'">
          <i>Обязанности:</i> 
          <ul>
            <li>Создание датасетов на основе необработанных данных из логов мобильного приложения.</li>
            <li>Обработка датасетов, добавление новых метрик.</li>
            <li>Создание моделей для машинного обучения.</li>
            <li>Исследование прогнозирующих моделей.</li>
            <li>Использование модели Маркова для прогнозирования действий пользователя в приложении.</li>
          </ul>
        </p>
        <p>
          <i>Used skills:</i> ExpressJS · Django · Flask · ML · Python · Pandas ·
          Catboost · SciKit Learn · Math Statistics · Scientific research
        </p>
      </div>

      <!-- Fullstack Developer -->
      <div class="work-title">
        <h2>Fullstack Developer</h2>
        <h3>Freelance</h3>
        <h3>2019</h3>
      </div>
      <div class="work-info">
        <p v-show="props.language == 'en'">
          <i>Responsibilities:</i> 
          <ul>
            <li>Developing a web application on the Mongo Express Vue Node stack.</li>
            <li>Creation of a server-side CRUD applicationы.</li>
            <li>Implementing SPA for selling services.</li>
            <li>Using AWS and Docker to deploy a microservice applications.</li>
          </ul>
        </p>
        <p v-show="props.language == 'ru'">
          <i>Обязанности:</i> 
          <ul>
            <li>Разработка веб-приложений на стеке Mongo Express Vue Node.</li>
            <li>Создание серверноых CRUD-приложений.</li>
            <li>Реализация SPA для продажи услуг.</li>
            <li>Использование AWS и Docker для развертывания микросервисноых систем.</li>
          </ul>
        </p>
        <p>
          <i>Used skills:</i> Express.js · Django · HTML · CSS · SASS · Docker ·
          Figma · SPA · AWS · Nginx · VueJS · NuxtJS · NodeJS · Python ·
          TypeScript · NestJS · JavaScript · Linux · Bash
        </p>
      </div>

      <!-- Frontend Developer -->
      <div class="work-title">
        <h2>Frontend Developer</h2>
        <h3>Freelance</h3>
        <h3>2018</h3>
      </div>
      <div class="work-info">
        <p v-show="props.language == 'en'">
          <i>Responsibilities:</i>
          <ul>
            <li>Developing web pages using Vue JS.</li>
            <li>Fixing bugs in the layout.</li>
            <li>Connecting frontend to backend using REST API.</li>
            <li>Using the concept of a SPA to implement a selling service.</li>
            <li>Deploying websites to AWS.</li>
          </ul>
        </p>
        <p v-show="props.language == 'ru'">
          <i>Обязанности:</i>
          <ul>
            <li>Разработка веб-страниц с использованием Vue JS.</li>
            <li>Исправление ошибок в макете.</li>
            <li>Подключение фронтенда к бэкенду с использованием REST API.</li>
            <li>Использование концепции SPA для реализации сервиса продажи.</li>
            <li>Развертывание веб-сайтов на AWS.</li>
          </ul>
        </p>
        <p>
          <i>Used skills:</i> HTML · CSS · SASS · Figma · Single Page
          Applications · Amazon Web Services (AWS) · Nginx · VueJS · Linux ·
          Bash
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

    ul
    {
      li{
        list-style: inside;
        list-style-type: circle;
      }
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
