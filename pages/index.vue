<template>
  <div class="static container bg-black max-w-none max-h-full text-white">
    <img
      class="cropped animate__animated headShake"
      src="@/assets/logo.png"
      alt="everlasting nothingness"
    />
    <audio
      id="alanwatts"
      controls
      class="absolute bottom-0"
      autoplay
      muted
      :src="require('@/assets/EVERYTHING.mp3')"
    ></audio>
  </div>
</template>

<script></script>

<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.cropped {
  object-fit: cover;
  height: 300px;
  width: 1080px;
}
</style>
