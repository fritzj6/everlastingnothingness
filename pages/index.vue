<template>
  <div class="static container bg-black max-w-none max-h-full text-white">
    <div class="flex flex-col font-mono">
      <p>everlasting</p>
      <p>nothingness</p>
    </div>

    <audio
      id="alanwatts"
      controls
      class="absolute bottom-0 right-0 border-0"
      autoplay
      muted
      :src="require('@/assets/EVERYTHING.mp3')"
    ></audio>
  </div>
</template>

<script>
export default {}
</script>

<style>
/* Sample `apply` at-rules with Tailwind CSS
.container {
@apply min-h-screen flex justify-center items-center text-center mx-auto;
}
*/
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

/* Specifies the size of the audio container */
audio {
  width: 115px;
  height: 25px;
}

audio::-webkit-media-controls-panel {
  /* -webkit-justify-content: center;
  height: 25px; */
}

audio::-webkit-media-controls-play-button {
  display: none;
}

/* Removes the timeline */
audio::-webkit-media-controls-timeline {
  /* display: none !important; */
}

/* Removes the time stamp */
audio::-webkit-media-controls-current-time-display {
  display: none;
}
audio::-webkit-media-controls-time-remaining-display {
  display: none;
}
</style>
