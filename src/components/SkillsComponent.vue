<template>
  <section id="skills">
    <div class="container">
      <h2 class="section-header">Skills</h2>
      <hr />
      <div class="space"></div>
      <div class="skills-section">
        <h2>Backend</h2>
        <div class="skills-list">
          <a href="https://www.javascript.com/" target="_blank" class="skill">
            <img src="../assets/js.png" alt="" />
            JavaScript
          </a>
          <a href="https://www.typescriptlang.org/" target="_blank" class="skill">
            <img src="../assets/ts.png" alt="" />
            TypeScript
          </a>
          <a href="https://nestjs.com/" target="_blank" class="skill">
            <img src="../assets/nest.png" alt="" />
            NestJS
          </a>
          <a href="https://expressjs.com/" target="_blank" class="skill">
            <img src="../assets/express.png" alt="" />
            ExpressJS
          </a>
          <a href="https://www.python.org/" target="_blank" class="skill">
            <img src="../assets/py.png" alt="" />
            Python
          </a>
          <a href="https://nodejs.org/" target="_blank" class="skill">
            <img src="../assets/node.png" alt="" />
            NodeJS
          </a>
          <a href="https://jestjs.io/" target="_blank" class="skill">
            <img src="../assets/jest.svg" alt="" />
            Jest
          </a>
          <a href="https://kafka.apache.org/" target="_blank" class="skill">
            <img src="../assets/kafka.png" alt="" />
            Kafka
          </a>
          <div class="skill">
            <img src="../assets/bash.png" alt="" />
            Unix Shell
          </div>
        </div>
      </div>
      <div class="space"></div>
      <div class="skills-section">
        <h2>Frontend</h2>
        <div class="skills-list">
          <a href="https://www.javascript.com/" target="_blank" class="skill">
            <img src="../assets/js.png" alt="" />
            JavaScript
          </a>
          <div class="skill">
            <img src="../assets/html.png" alt="" />
            HTML
          </div>
          <div class="skill">
            <img src="../assets/css.png" alt="" />
            CSS
          </div>
          <a href="https://sass-lang.com/" target="_blank" class="skill">
            <img src="../assets/sass.png" alt="" />
            Sass
          </a>
          <a href="https://vuejs.org/" target="_blank" class="skill">
            <img src="../assets/vue.png" alt="" />
            Vue
          </a>
          <a href="https://vuex.vuejs.org/" target="_blank" class="skill">
            <img src="../assets/vuex.png" alt="" />
            Vuex
          </a>
          <a href="https://nuxtjs.org/" target="_blank" class="skill">
            <img src="../assets/nuxt.avif" alt="" />
            Nuxt
          </a>
          <a href="https://vitejs.dev/" target="_blank" class="skill">
            <img src="../assets/vite.png" alt="" />
            Vite
          </a>
          <a href="https://getbootstrap.com/" target="_blank" class="skill">
            <img src="../assets/bs.png" alt="" />
            Bootstarp
          </a>
          <a href="https://www.figma.com/" target="_blank" class="skill">
            <img src="../assets/figma.png" alt="" />
            Figma
          </a>
        </div>
      </div>
      <div class="space"></div>
      <div class="skills-section">
        <h2>Storage</h2>
        <div class="skills-list">
          <a href="https://mongodb.org" target="_blank" class="skill">
            <img src="../assets/mongo.svg" alt="" />
            MongoDB
          </a>
          <a href="https://www.postgresql.org/" target="_blank" class="skill">
            <img src="../assets/postgres.png" alt="" />
            PostgreSQL
          </a>
          <a href="https://min.io/" target="_blank" class="skill">
            <img src="../assets/minio.png" alt="" />
            MinIO
          </a>
          <a href="https://aws.amazon.com/ru/s3/" target="_blank" class="skill">
            <img src="../assets/s3.svg" alt="" />
            S3 Bucket
          </a>
          <a href="https://redis.io/" target="_blank" class="skill">
            <img src="../assets/redis.jpg" alt="" />
            Redis
          </a>
        </div>
      </div>

      <div class="space"></div>
      <div class="skills-section">
        <h2>Familiar with</h2>
        <div class="skills-list">
          <a href="https://git-scm.com/" target="_blank" class="skill">
            <img src="../assets/git.png" alt="" />
            Git
          </a>
          <a href="https://www.docker.com/" target="_blank" class="skill">
            <img src="../assets/docker.png" alt="" />
            Docker
          </a>
          <a href="https://www.jenkins.io/" target="_blank" class="skill">
            <img src="../assets/jenkins.png" alt="" />
            Jenkins</a
          >
          <a href="https://www.keycloak.org/" target="_blank" class="skill">
            <img src="../assets/keycloak.png" alt="" />
            Keycloak
          </a>
          <div class="skill">IoT</div>
          <div class="skill">HTTP</div>
          <div class="skill">MQTT</div>
          <div class="skill">SSH</div>
        </div>
      </div>

      <div class="space"></div>
      <div class="skills-section">
        <h2>Used principles</h2>
        <div class="skills-list">
          <div class="skill">REST</div>
          <div class="skill">Microservice</div>
          <div class="skill">Clean architecture</div>
          <div class="skill">TDD</div>
          <div class="skill">Domain-Driven Design</div>
          <div class="skill">SPA</div>
          <div class="skill">SSR</div>
          <div class="skill">MVC</div>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped lang="scss">
#skills {
  margin-top: -20px;
  background: var(--text);
  flex-direction: column;
  justify-content: center;
  width: 100vw;
  color: var(--bg);
  padding-bottom: 20px;

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

  .skills-section {
    h2 {
      font: 1.7em "Jura";
    }
    .skills-list {
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
  #skills {
    h2 {
      font-size: 1.2em;
    }

    p {
      width: 100%;
      font-size: 1em;
    }
    .skills-section {
      h2 {
        font: 1em "Jura";
      }
      .skills-list {
        font-size: 0.7rem;
      }
    }
  }
}
/* Min-width: 320px (smaller phone viewpoints) */
@media only screen and (min-width: 320px) {
  #skills {
    h2 {
      font-size: 1.5em;
    }
    p {
      width: 100%;
      font-size: 1em;
    }

    .skills-section {
      h2 {
        font: 1.2em "Jura";
      }
      .skills-list {
        font-size: 0.7rem;
      }
    }
  }
}

/* Min-width: 480px (small devices and most phones) */
@media only screen and (min-width: 480px) {
  #skills {
    h2 {
      font-size: 1.5em;
    }
    p {
      width: 100%;
    }

    .skills-section {
      .skills-list {
        font-size: 0.8rem;
      }
    }
  }
}

/* Min-width: 768px (most tablets) */
@media only screen and (min-width: 768px) {
  #skills {
    .wave {
      margin-top: -100px;
    }
    h2 {
      font-size: 2em;
    }
    .skills-section {
      .skills-list {
        font-size: 1rem;
      }
    }
  }
}

/* Min-width: 992px (smaller desktop viewpoints) */
@media only screen and (min-width: 992px) {
  #skills {
    h2 {
      font-size: 2.5em;
    }
    p {
      width: 80%;
    }
  }
}
</style>
