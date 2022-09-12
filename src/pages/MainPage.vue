<template>
  <div class="container">
    <video
          src="~assets/backgroundVideo.mp4" muted
          autoplay
          loop />
  </div>

  <!-- Botones aqui -->

  <h1 class="text-h3 centerText absolute-center matriverRegularFont">I am Juanma</h1>


  <h2>dasndonadnasn</h2>
</template>

<script>
export default {

}
</script>

<style scoped lang="scss">


.centerText {
  // background-color: red;
  font-size: 70px;
  color: $vue-primary;
  text-align: center;
}

.container {
  height: 100vh;
  width: 100%;
}

video {
  height: 100%;
  width: 100%;
  object-fit: fill;
}

</style>