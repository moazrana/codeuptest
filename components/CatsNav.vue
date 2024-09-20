<template>
  <div id="cats-nav">
    <div id="list">
        <div v-for="cat in cats" :key="cat" @click="getItems(cat)">
            {{ cat }}
        </div>
    </div>
  </div>
</template>

<script setup>
import { ref, onMounted } from 'vue'
import { defineEmits } from 'vue'

const cats = ref(null)

onMounted(async () => {
  const response = await fetch('https://fakestoreapi.com/products/categories')
  const json = await response.json()
  cats.value=json
})

const emit = defineEmits(['gotItems'])
const getItems=async (cat)=>{
    const response = await fetch('https://fakestoreapi.com/products/category/'+cat)
    const json = await response.json()
    emit('gotItems',json)
}
</script>
<style>
    #list{
        display: flex;
        flex-direction:row ;
        justify-content: space-evenly;
    }
</style>