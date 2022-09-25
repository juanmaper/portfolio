<template>
  
  <transition
    appear
    enter-active-class="animated fadeInUp"
    leave-active-class="animated rotateOut"
  >
  <h1 class="headerText text-center matriverRegularFont">{{ $t('aboutMe.title') }}</h1>

</transition>

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