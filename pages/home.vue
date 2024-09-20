<template>
  <div id="main-div">
    <hero-banner></hero-banner>
    <cats-nav @gotItems="items=$event"/>
    <div id="items">
      <item v-for="item in items" :key="item.id" :item="item.title" :image="item.image" :price="item.price"/>
    </div>
  </div>
</template>

<script>
import HeroBanner from '../components/HeroBanner.vue'
import CatsNav from '../components/CatsNav.vue'
export default {
  components:{HeroBanner,CatsNav},
  data(){
    return{
      items:[]
    }
  }
}
</script>

<style scoped>
 #items{
  display: flex;
  justify-content: space-around;
 }

</style>