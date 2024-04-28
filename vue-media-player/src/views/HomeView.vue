<template>
  <main>
    <h1 class="fs-medium-lg fw-large text-center mx-auto col-lg-9 col-12 px-0 line-sm">Listen to<br> your
      favorite
      songs.
    </h1>
    <p class="text-center mt-4 mb-5 mx-auto col-lg-9  col-12 px-0 fs-medium fw-medium line-sm">Stream all your songs and
      audio
      files
      in one
      place,
      and
      experience
      new
      emotions.
    </p>

    <div class="songs-listcard mx-auto">

      <div class="music-card" style=" margin-left: -28% !important;
      padding:25px;">
        <img src="/cdn/images/music-card-01.png" class="song-cover rounded-4" alt="">
      </div>

      <div class="music-card" style=" margin-left: -18% !important;
      padding: 15px;">
        <img src="/cdn/images/music-card-02.png" class="song-cover rounded-4" alt="">
      </div>

      <div class="music-card" style="
      padding:0px;">
        <img src="/cdn/images/music-card-03.png" class="song-cover rounded-4" alt="">
      </div>

      <div class="music-card" style=" margin-left: 18% !important;
      padding: 15px;">
        <img src="/cdn/images/music-card-04.png" class="song-cover rounded-4" alt="">
      </div>

      <div class="music-card" style=" margin-left: 28% !important;
      padding: 25px;">
        <img src="/cdn/images/music-card-05.png" class="song-cover rounded-4" alt="">
      </div>


    </div>
  </main>
</template>

<script>
export default {
}
</script>

<style scoped>
.songs-listcard {
  width: 100%;
  height: 100%;
  position: relative;
  top: 115px;
}

.songs-listcard .music-card {
  overflow: hidden;
  width: 250px !important;
  height: 250px !important;
  max-height: 250px !important;
  min-width: 50px;
  min-height: 50px;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}

.songs-listcard .music-card img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  object-position: center;
}


/* Front-Displacement */
.songs-listcard .music-card:nth-of-type(3) {
  z-index: 3;
}

.songs-listcard .music-card:is(:nth-of-type(1), :nth-of-type(5)) {
  z-index: 1;
}

.songs-listcard .music-card:is(:nth-of-type(2), :nth-of-type(4)) {
  z-index: 2;
}
</style>
