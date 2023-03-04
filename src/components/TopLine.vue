<script setup>
import { onMounted, reactive} from 'vue'
import NavIcon from './svg/NavIcon.vue';
import CloseIcon from './svg/CloseIcon.vue';

const state = reactive({
  hide_nav: true,
  toggler_text: "NAVIGATIOn"
});

const toggleNav = () => {
  state.hide_nav = !state.hide_nav
  const topline = document.getElementById("topline")
  const nav = document.getElementsByTagName("nav")[0]
  if(state.hide_nav == false){
    nav.style.display = "flex";
    topline.style.background = "#121212dd";
  }else{
    nav.style.display = "none";
    topline.style.background = "transparent";
  }
}
    
    


window.addEventListener('scroll', onScroll);
function onScroll() {
  const scrollTop = window.pageYOffset;
  if (scrollTop > 20){  
    document.getElementById("topline").style.background = "#121212";
  } else {
    document.getElementById("topline").style.background = "transparent";
  }
}
</script>

<template>
  <div id="topline">
    <div class="topline-content container">
      <h2 class="logo">
        Cawa
      </h2>
      <nav :class="{'hidden': hide_nav}">
        <a href="#">Home</a>
        <a href="#">About</a>
        <a href="#">Experiebce</a>
        <a href="#">Skills</a>
        <a href="#">Contact me</a>
      </nav>
      <div id="nav-toggler" @click="toggleNav">
        <CloseIcon :class="{'faded':state.hide_nav}"></CloseIcon>
        <NavIcon :class="{'faded':!state.hide_nav}"></NavIcon>
      </div>
    </div>
  </div>
  <div class="space"></div>
  <div class="space"></div>
</template>

<style scoped lang="scss">

#topline{
  display: flex;
  position: fixed;
  top:0;
  left:0;
  justify-content: center;
  height: 4em;
  width: 100vw;
  transition: background 0.3s ease;
  // border: 1px solid #fff;
}

.topline-content{
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.logo{
  font-family: "HachiMaru";
  padding: 0.5em 0;
  margin: 0;
}

nav{
  font-family: "Jost";
  font-weight: 900;
  display: flex;
  // display: none;
  flex-direction: column;
  position: fixed;
  top: 4em;
  left :0;
  width: 100vw;
  min-height: 100vh;
  background: #121212dd;
  justify-content: center;
  align-items: center;

  &.hidden{
    display: none !important;
  }

  a {
    padding: 1em;
    display: flex;
    width: fit-content;
    transition: all 0.1s ease-in;
    // border:1px solid #fff

    &:hover{
      transform: scale(1.2);
      color: var(--accent);
      // color: #00a3c0;
    }
  }
}

#nav-toggler {
  display: flex;
  position: relative;
  cursor: pointer;
  
  .faded{
    position: absolute;
    opacity: 0;
  }
}

a{
  text-transform: uppercase;
  color:#fafafa;
 

}

/* Min-width: 320px (smaller phone viewpoints) */
@media only screen and (min-width: 320px) {
 nav{
    display: none;

 }
}

/* Min-width: 480px (small devices and most phones) */
@media only screen and (min-width: 480px) {
}

/* Min-width: 768px (most tablets) */
@media only screen and (min-width: 768px) {
 
}

/* Min-width: 992px (smaller desktop viewpoints) */
@media only screen and (min-width: 992px) {
  #nav-toggler {
    display: none;
  }
  nav{
    display: flex !important;
    font-weight: 900;
    gap: 1em;
    flex-direction: row;
    position: relative;
    width: auto;
    min-height: 2em;
    padding: 0;
    background: none;
    top: 0;
    &.hidden{
    display: none !important;
  }

    a{
      &:hover{
        transform: scale(1);
      }
    }
  }
}

/* Min-width: 1200px (large devices and wide screens */
@media only screen and (min-width: 1200px) {

}

</style>
