<template>
  <div>
    <NuxtRouteAnnouncer />
    <nav-bar/>
    <NuxtPage />
    <!-- <NuxtWelcome /> -->
  </div>
</template>

<script>
import NavBar from './components/Nav.vue'
export default {
  components:{NavBar}
}
</script>

<style>

</style>
