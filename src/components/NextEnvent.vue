<template>

  <div class="next-event-section">

    <div class="row m-0 p-0">
      <div class="col-6 m-0 p-0">
        <div class="left"></div>
      </div>
      <div class="col-6 m-0 p-0">
        <div class="right">
          <div class="font-bold">Prochain événement</div>
          <div class="title">
            <div class="main-title neon-text">FULL MOON</div>
            <div class="subtitle">story</div>
          </div>
          <div>
            <div>MERCREDI 30 AVRIL 2025</div>
            <div class="important">6 places restantes</div>
          </div>

          <div>
            <button class="btn-reserve">Je réserve ma soirée!</button>
          </div>
        </div>
      </div>
    </div>

  </div>

</template>

<style scoped>
.next-event-section{
  width: 100dvw;
  height: 100dvh;
  background-color: #000000;
  font-size: 2.5rem;
  color: #dad4d4;
  text-align: center;
}
.left{
  background-image: url("/src/assets/image/hero_01.png");
}

.right{
  background-image: url("/src/assets/image/dead_man.webp");
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  gap: 4rem;
  background-position: right;
  position: relative;
  z-index: 0;
  font-family: FaceOfYourFear, sans-serif;
}
.right:after{
  content: "";
  position: absolute;
  background-color: black;
  min-width: 100%;
  min-height: 100%;
  opacity: 0.8;
  z-index: -1;
}

.left, .right{
  background-color: coral;
  background-size: cover;
  min-height: 100dvh;
  width: 100%;
}

.btn-reserve{
  margin-top: 2rem;
  background: rgb(255,72,0);
  background: linear-gradient(90deg, rgb(253, 51, 50) 0%, rgb(253, 143, 76) 100%);
  padding: 1.3rem 5rem;
  border-radius: 38px;
}



.main-title{
  font-family: 'Rockwill', sans-serif;
  font-size: 6rem;
  color: rgb(218, 185, 121);
  transform: scaleY(1.8);
}

.neon-text {
  color: rgb(218, 185, 121);
  text-shadow:
    0 0 2px rgba(218, 185, 121, 0.4),
    0 0 4px rgba(218, 185, 121, 0.3),
    0 0 6px rgba(255, 220, 160, 0.2),
    0 0 8px rgba(255, 235, 190, 0.2);
  animation: glow 8s ease-in-out infinite;
}

@keyframes glow {
  0% {
    text-shadow:
      0 0 2px rgba(218, 185, 121, 0.4),
      0 0 4px rgba(218, 185, 121, 0.3),
      0 0 6px rgba(255, 220, 160, 0.2),
      0 0 8px rgba(255, 235, 190, 0.2);
  }
  50% {
    text-shadow:
      0 0 8px rgba(218, 185, 121, 0.6),
      0 0 15px rgba(218, 185, 121, 0.5),
      0 0 20px rgba(255, 220, 160, 0.3),
      0 0 30px rgba(255, 235, 190, 0.4);
  }
  100% {
    text-shadow:
      0 0 2px rgba(218, 185, 121, 0.4),
      0 0 4px rgba(218, 185, 121, 0.3),
      0 0 6px rgba(255, 220, 160, 0.2),
      0 0 8px rgba(255, 235, 190, 0.2);
  }
}





.subtitle{
  font-family: 'ScreamAgain', sans-serif;
  color: rgb(255,72,0);
  font-size: 4rem;
}

.important {
  color: rgb(253, 49, 49);
  animation: beat 1.5s ease-in-out infinite,  beat-color 1.5s ease-in-out infinite;
}

@keyframes beat {
  0%, 50%, 100% { transform: scale(1, 1); }
  30%, 80% { transform: scale(0.97, 0.96); }
}

@keyframes beat-color {
  0%, 50%, 100% { color: rgb(253, 49, 49); }
  30%, 80% { color: rgb(204, 11, 4); }
}








</style>
<script setup lang="ts">
</script>
