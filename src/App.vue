<script setup>
function playClickSound(){
  const audio = new Audio("/public/sound/mouse_click.wav");
  audio.play();
}


</script>

<template>
  <div class="wrapper">
    <div class="inner_column">
      <div class="header">
        <div class="dvdGif"></div>
        <h1>neveroyatno original'no</h1>
      </div>
      <div class="retro-container">
        <button class="retro-btn" @click="playClickSound"> Click here</button>
      </div>
      <div class="bgGif"></div>
    </div>
  </div>


</template>

<style scoped> </style>
