<template>
    <div id="main-div">
        <div class="card">
        <img :src="image" :alt="item">
        <h3>{{ item }}</h3>
        <p class="price">${{ price }}</p>
        <button @click=addToCart()>Add to Cart</button>
    </div>
    </div>
</template>

<script setup>
    const props=defineProps({
        item:{
            type:String,
            required:true
        },
        image:{
            type:String,
            required:true
        },
        price:{
            type:String,
            required:true
        }
    })

    const addToCart=()=>{
        localStorage.setItem()
    }
</script>

<style scoped>
* {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    #main-div {
      font-family: Arial, sans-serif;
      background-color: #f4f4f4;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
    }

    .card {
      width: 300px;
      background-color: #fff;
      border-radius: 10px;
      box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
      padding: 20px;
      text-align: center;
      height: inherit;
    }

    .card img {
      max-width: 100%;
      height: auto;
      border-radius: 8px;
    }

    .card h3 {
      font-size: 18px;
      margin: 15px 0 10px;
    }

    .card p {
      color: #888;
      font-size: 14px;
    }

    .card .price {
      font-size: 20px;
      font-weight: bold;
      margin: 10px 0;
    }

    .card button {
      background-color: #000;
      color: #fff;
      border: none;
      border-radius: 5px;
      padding: 10px;
      font-size: 16px;
      cursor: pointer;
      width: 100%;
    }

    .card button:hover {
      background-color: #444;
    }
</style>