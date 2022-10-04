<template>
  
  <div class="column items-center" style="margin-top: 200px;">
    <q-intersection transition="fade" :threshold="1" style="width: 100%; height: 200px;" once>
    

      <h1  class="headerText text-center matriverRegularFont">{{ $t('aboutMe.title') }}</h1>

    
    
    </q-intersection>
  </div>
  
  <div class="column items-center">

    <q-intersection transition="fade" :threshold="1" style="width: 70%; height: 200px;" once>
    
      
          <p class="text-center">{{ $t('aboutMe.text') }}</p>
        
    </q-intersection>
  </div>


</template>

<script>
export default {

}
</script>

<style scoped lang="scss">


</style>