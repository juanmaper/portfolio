<template>
  
  <q-intersection transition="fade" :threshold="1" >
    

    <h1  class="headerText text-center matriverRegularFont">{{ $t('aboutMe.title') }}</h1>

    
    
  </q-intersection>
  
  <q-intersection transition="fade" :threshold="1" >
  
    <div class="column items-center">
        <p class="col">{{ $t('aboutMe.text') }}</p>
      </div>
  </q-intersection>


</template>

<script>
export default {

}
</script>

<style scoped lang="scss">

h1 {
  margin-top: 300px;
}

p {
  margin-top: 50px;
}

</style>