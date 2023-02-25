<script setup>
import { ref } from 'vue'
const count = ref(0)
window.addEventListener('scroll', onScroll);

function onScroll() {
  const scrollTop = window.pageYOffset;
  if (scrollTop > 20)
{  document.getElementById("topline").style.background = "#121212";}
  else {
    document.getElementById("topline").style.background = "transparent";
  }
}
</script>

<template>
  <div id="topline">
    <div class="topline-content container">
      <h2 class="logo">
        CAWA
      </h2>
      <nav>
        <a href="#">Home</a>
        <a href="#">About</a>
        <a href="#">Experiebce</a>
        <a href="#">Skills</a>
        <a href="#">Contact me</a>
      </nav>
    </div>
  </div>
</template>

<style scoped lang="scss">

#topline{
  display: flex;
  position: fixed;
  top:0;
  left:0;
  justify-content: center;
  width: 100vw;
  opacity: 1;
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
  gap: 1em;
}

a{
  text-transform: uppercase;
  color:#fafafa
}


</style>
