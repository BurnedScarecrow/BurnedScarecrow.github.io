<script setup>
import { ref } from "vue";
const lang = ref("en");
</script>

<template>
  <section id="about">
    <div class="container">
      <h2 class="section-header">
        About me
        <span class="lang" @click="lang = lang == 'ru' ? 'en' : 'ru'">{{ lang == "ru" ? "en" : "ru" }}</span>
      </h2>
      <div class="space"></div>
      <div class="section-content">
        <p v-show="lang == 'ru'">
          Как разработчик с <span class="accent">3-летним профессиональным опытом</span>, я увлечен
          разработкой иновационных решений современных проблем. Последние 5 лет обучения стали для меня
          прекрасной возможностью попробовать себя в различных сферах IT, включая как популярыне
          <span class="accent">Backend и Frontend</span>, так и специфичные, например информационная
          безопасность и реверс-инжиниринг.
        </p>

        <p v-show="lang == 'ru'">
          Сейчас я <span class="accent">работаю над дипломной работой</span> о методах обхода блокировок
          интернет-ресурсов и интернет-цензуры путем проксирования, туннелирования и обфускации трафика, так
          как
          <span class="accent">я за свободу в интернете.</span>
        </p>
        <p v-show="lang == 'ru'">
          В своей карьере <span class="accent">я стремлюсь улучшить свои технические навыки</span> в области
          серверной разработки, проектирования программного обеспечения, тестирования и внедрения надежных и
          безопасных систем. На данный момент я
          <span class="accent">заинтересован в изучении кластерных и облачных решений</span> для
          масштабируемых высокопроизводительных приложений. Мне очень нравится создавать программные продукты,
          которые прекрасны как на взгляд пользователей, так и разработчиков.
          <span class="accent">Давайте создадим что-нибудь вместе!</span>
        </p>
        <p v-show="lang == 'en'">
          As a software engineer with <span class="accent">3 years of professional experience</span>, I am
          passionate about developing innovative solutions that solve complex problems. Last 5 years of
          studying have become for me a great opportunity to try myself in lots of fields of IT including
          popular <span class="accent">Backend and Frontend</span>, and specific like information security and
          reverse engineering.
        </p>
        <p v-show="lang == 'en'">
          Nowadays I am <span class="accent">working on my graduation work</span> about methods for bypassing
          blocking of Internet resources and Internet censorship by traffic proxying, tunneling and
          obfuscation, as <span class="accent">I am for freedom in the internet.</span>
        </p>
        <p v-show="lang == 'en'">
          In my career I am <span class="accent">looking to enhance my technical skills</span> in backend,
          software design, testing and implementing reliable and secure systems. For now,
          <span class="accent">I am interested in studying cluster and cloud solutions</span> for scalable
          high-performance applications. I extremely like creating software products that are wonderful both
          for a glance of users and developers.
          <span class="accent">Let's create something togeather!</span>
        </p>
      </div>
    </div>
    <svg class="wave" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320">
      <path
        fill="#fafafa"
        fill-opacity="1"
        d="M0,32L80,42.7C160,53,320,75,480,117.3C640,160,800,224,960,213.3C1120,203,1280,117,1360,74.7L1440,32L1440,320L1360,320C1280,320,1120,320,960,320C800,320,640,320,480,320C320,320,160,320,80,320L0,320Z"
      ></path>
    </svg>
  </section>
</template>

<style scoped lang="scss">
#about {
  margin-top: -1px;
  margin-bottom: 0;
  padding-bottom: 0;
  box-sizing: border-box;
  background: var(--bg);
  flex-direction: column;
  justify-content: center;
  width: 100vw;
  color: var(--text);

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

  .wave {
    margin: 0;
    padding: 0;
    margin-bottom: -6px;
    box-sizing: border-box !important;
  }
}

/* Min-width: 320px (smaller phone viewpoints) */
@media only screen and (max-width: 320px) {
  #about {
    h2 {
      font-size: 1.2em;
    }

    p {
      width: 100%;
      font-size: 1em;
      margin-bottom: 2em;
    }
  }
}
/* Min-width: 320px (smaller phone viewpoints) */
@media only screen and (min-width: 320px) {
  #about {
    h2 {
      font-size: 1.5em;
    }
    p {
      width: 100%;
      font-size: 1em;
      margin-bottom: 2em;
    }
  }
}

/* Min-width: 480px (small devices and most phones) */
@media only screen and (min-width: 480px) {
  #about {
    h2 {
      font-size: 1.5em;
    }
    p {
      width: 100%;
      margin-bottom: 2em;
    }
  }
}

/* Min-width: 768px (most tablets) */
@media only screen and (min-width: 768px) {
  #about {
    .wave {
      margin-top: -100px;
    }
    h2 {
      font-size: 2em;
    }
    .section-content {
      p {
        width: 80%;
        margin-bottom: 3em;
        font-size: 1.2em;
        &:nth-child(1) {
          margin-left: 0%;
        }
        &:nth-child(2) {
          margin-left: 10%;
        }
        &:nth-child(3) {
          margin-left: 20%;
        }
        &:nth-child(4) {
          margin-left: 0%;
        }
        &:nth-child(5) {
          margin-left: 10%;
        }
        &:nth-child(6) {
          margin-left: 20%;
        }
      }
    }
  }
}

/* Min-width: 992px (smaller desktop viewpoints) */
@media only screen and (min-width: 992px) {
  #about {
    h2 {
      font-size: 2.5em;
    }
    p {
      width: 80%;
    }
  }
}
</style>
