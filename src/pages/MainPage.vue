<template>
  <div class="container">
    <video
          src="~assets/backgroundVideo.mp4" muted
          autoplay
          loop />
  </div>

  <div class="row">
    <div class="absolute-right q-pa-md q-gutter-sm col-4">
      <q-btn flat style="color: #FF0080" label="Fuchsia Flat" />
      <q-btn flat unelevated no-caps text-color="vue-primary" :label="$t('buttons.aboutMe')" />
      <q-btn flat unelevated no-caps :label="$t('buttons.projects')" />
      <q-btn flat unelevated no-caps :label="$t('buttons.contact')" />
    </div>
  </div>
    
      
    

  <q-select
    v-model="locale"
    :options="localeOptions"
    label="Quasar Language"
    dense
    borderless
    emit-value
    map-options
    options-dense
    style="min-width: 150px"
  />

  <p>{{ $t("failed") }}</p>

  <textarea v-model="locale"></textarea>

  <!-- Botones aqui -->

  <h1 class="text-h3 centerText absolute-center matriverRegularFont">I am Juanma</h1>


  <h2>dasndonadnasn</h2>
</template>

<script>
import { useI18n } from 'vue-i18n'

export default {

  setup() {

    const { locale } = useI18n({ useScope: 'global' })
    return {
      locale,
      localeOptions: [
        { value: 'en-US', label: 'English' },
        { value: 'es-ES', label: 'Spanish' }
      ]
    }
  
  }

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

.redBackground {
  background-color: red;
}

</style>