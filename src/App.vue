<script >
export default {
  data() {
    return {
      games: [],
      givenGame: null
    };
  },
  mounted() {
    fetch('/games.json')
        .then(res => res.json())
        .then(data => {
          this.games = data;
          console.log("Загруженные игры:", this.games);
        });
  },
  methods: {
    playClickSound(){
    const audio = new Audio("/sound/mouse_click.wav");
    audio.play();
    },
    getRandomGame(){
      let index = Math.ceil(Math.random() * this.games.length);
      this.givenGame = this.games[index];
    }
  }
}


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
