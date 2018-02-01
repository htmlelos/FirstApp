<template>
<div class="media-player">
  <div class="progress">
    <span>2:24</span>
    <progress value="50" max="100">50%</progress>
    <span>4:13</span>
  </div>
  <div class="info">
    <figure class="info_cover">
      <img src="https://www.amazon.co.uk/Counting-Down-Days-Natalie-Imbruglia/dp/B0007YH6AG" alt="">
    </figure>
    <div class="info_data">
      <div class="title">Counting Down The Days</div>
      <div class="artist">Natalie Imbruglia</div>
      <div class="album">Counting Down The Days</div>
    </div>
  </div>
  <div class="controls">
    <a class="player-btn" href="#"><i class="fa fa-refresh"></i></a>
    <a class="player-btn" href="#"><i class="fa fa-step-backward"></i></a>
    <a class="player-btn" href="#"><i class="fa fa-play"></i></a>
    <a class="player-btn" href="#"><i class="fa fa-step-forward"></i></a>
    <audio id="track" src="static/Aerosmith%20-%20Crazy"></audio>
  </div>
</div>
</template>
<script>
export default {
  name: 'MediaPlayer',
  data () {
    return {
      currentMedia: 'Test.mp3'
    }
  },
  methods: {
    play: () => {
      console.log('PLAY')
    },
    pause: () => {
      console.log('PAUSE')
    },
    stop: () => {
      console.log('STOP')
    },
    backward: () => {
      console.log('BACKWARD')
    },
    forward: () => {
      console.log('FORWARD')
    }
  }
}
</script>
<style>
.progress {
  display: flex;
  justify-content: space-around;
  align-items: center;
}
.info {
  display: flex;
}
.info .title {
  font-size: 1.5em;
}
.info .artist {
  font-size: 1em;
}
.controls {
  padding: 0.5em;
  /* border: 1px solid black; */
  display: flex;
  justify-content: center;
  align-items: center;
}
.player-btn {
  display: flex;
  justify-content: center;
  align-items: center;
  border: 2px solid black;
  border-radius: 50%;
  width: 1.5em;
  height: 1.5em;
  text-decoration: none;
  padding: 0.5em;
  margin: 0.5em;
}

.player-btn:hover {
  background: blue;
  color: white;
}
</style>
