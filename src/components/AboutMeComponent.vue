<template>
  
  <q-intersection v-for="i in 60" :key="i" transition="fade" style="width: 200px; height:200px; margin-top:200px" 
    :threshold="1" once>
    

    <h1  class="headerText text-center matriverRegularFont">{{ $t('aboutMe.title') }}</h1>

  </q-intersection>
  


</template>

<script>
export default {

}
</script>

<style scoped lang="scss">

h1 {
  margin-top: 200px;
}

</style>