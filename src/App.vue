<script setup>
function playClickSound(){
  const audio = new Audio("/sound/mouse_click.wav");
  audio.play();
}
</script>

<template>
  <div id="wrapper">
    <div id="main_column">
      <div id="library" class="menu_bar">
        <span class="menu_item">Library</span>
      </div>
      <div class="retro-container">
        <button class="retro-btn" @click="playClickSound"> Click here</button>
      </div>

      <div id="bgGif"></div>
    </div>
  </div>


</template>

<style scoped> </style>
