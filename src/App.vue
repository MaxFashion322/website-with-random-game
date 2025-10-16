<script setup>
// function playClickSound(){
//   const audio = new Audio("/sound/mouse_click.wav");
//   audio.play();
// }
const playClickSound = () => new Audio("/sound/mouse_click.wav").play()




</script>

<template>
  <div id="wrapper">
    <div id="main">
      <div class="menu_bar">
        <div class="menu_item" @click="playClickSound">Library </div>
        <div class="menu_item" @click="playClickSound">List of Games </div>
      </div>

      <h1 class="main_title">BROTHER YOU CAN'T DECIDE, WHICH GAME TO PLAY???🎮
        <br>
        <br>well...
        <br>
        <br> press the button, maybe it helps 🤔
      </h1>

      <div class="retro_container">
        <button class="retro_btn" @click="playClickSound"> Click here</button>
      </div>

      <div id="bg_gif"></div>
    </div>
  </div>

  <div id="bg"></div>
</template>

<style scoped> </style>
