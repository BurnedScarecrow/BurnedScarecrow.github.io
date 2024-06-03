<script setup>
import { defineProps, defineEmits, ref } from "vue";

const props = defineProps({
  language: {
    type: String,
    required: true,
  },
});

const emit = defineEmits(["languageChanged"]);

const changeLanguage = () => {
  emit("languageChanged");
};
</script>

<template>
  <section id="about">
    <div class="container">
      <h2 class="section-header">
        About me
        <span class="lang" @click="changeLanguage">{{
          props.language == "ru" ? "en" : "ru"
        }}</span>
      </h2>
      <div class="space"></div>
      <div class="section-content">
        <p v-show="props.language == 'ru'">
          <span class="accent">С 2020 года</span> я профессионально занимаюсь
          разработкой программного обеспечения и в настоящее время работаю
          <span class="accent">ведущим инженером-программистом</span>,
          специализируясь на разработке и поддержке бэкенда. Мой опыт охватывает
          <span class="accent"
            >различные аспекты IT, включая фронтенд, бэкенд</span
          >, информационную безопасность, реверс-инжиниринг и машинное обучение.
        </p>

        <p v-show="props.language == 'ru'">
          Недавно я завершил обучение и успешно
          <span class="accent">защитил дипломную работу</span> по специальности
          "Информационная безопасность", в которой исследовал
          <span class="accent"
            >методы обхода блокировок интернет-ресурсов и интернет-цензуры</span
          >
          с использованием проксирования, туннелирования и обфускации трафика.
          Это исследование подчеркнуло мою
          <span class="accent">приверженность свободе интернета.</span>
        </p>
        <p v-show="props.language == 'ru'">
          В своей карьере я стремлюсь совершенствовать навыки в разработке
          программного обеспечения,
          <span class="accent"
            >проектировании систем и создании масштабируемых
            высокопроизводительных приложений</span
          >. Мне нравится разрабатывать программные продукты, которые радуют как
          пользователей, так и разработчиков.
          <span class="accent"
            >Давайте создадим что-то удивительное вместе!</span
          >
        </p>
        <p v-show="props.language == 'en'">
          <span class="accent">Since 2020,</span> I have been professionally
          engaged in software development and currently work as a
          <span class="accent">lead software engineer</span>, specializing in
          <span class="accent">backend development</span> and support. My
          <span class="accent">experience covers various aspects of IT,</span>
          including frontend, backend, information security, reverse
          engineering, and machine learning.
        </p>
        <p v-show="props.language == 'en'">
          Recently, I completed my studies and successfully
          <span class="accent">defended my thesis</span>
          in "Information Security," in which I investigated methods for
          <span class="accent"
            >bypassing internet resource blocks and censorship</span
          >
          using proxying, tunneling, and traffic obfuscation. This research
          underscored my
          <span class="accent">commitment to internet freedom.</span>
        </p>
        <p v-show="props.language == 'en'">
          In my career, I strive to enhance my skills in software development,
          system design, and the creation of
          <span class="accent">scalable high-performance applications</span>. I
          enjoy developing software products that delight both users and
          developers.
          <span class="accent">Let's create something amazing together!</span>
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
