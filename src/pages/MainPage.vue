<template>
  <div class="container">
    <video
          src="~assets/backgroundVideo.mp4" muted
          autoplay
          loop />
  </div>

  <div class="row">
    <div class="absolute-right q-pa-md q-gutter-sm col-5">
      <q-btn no-caps flat style="color: #FF0080" label="Fuchsia Flat" />
      <q-btn no-caps color="white" text-color="black" :label="$t('buttons.aboutMe')" />
      <q-btn no-caps color="primary" :label="$t('buttons.projects')" />
      <q-btn flat no-caps color="secondary" :label="$t('buttons.contact')" />
      <q-icon name="flag" color="white" size="32px"/>
      <q-icon name="flag" color="blue" size="32px"/>
    </div>
  </div>
    
      
    

  <!-- <q-select
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

  <textarea v-model="locale"></textarea> -->

  <!-- Botones aqui -->

  <h1 class="headerText absolute-center matriverRegularFont">I am Juanma</h1>


  <AboutMeComponent />
</template>

<script>
import { useI18n } from 'vue-i18n'
import AboutMeComponent from '../components/AboutMeComponent.vue'

export default {
    setup() {
        const { locale } = useI18n({ useScope: "global" });
        return {
            locale,
            localeOptions: [
                { value: "en-US", label: "English" },
                { value: "es-ES", label: "Spanish" }
            ]
        };
    },
    components: { AboutMeComponent }
}
</script>

<style scoped lang="scss">

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