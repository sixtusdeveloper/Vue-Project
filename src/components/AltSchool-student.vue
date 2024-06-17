<template>
    <!-- <h1>{{ msg }}</h1> -->
    <div class="inventory-container">
      <h2>Inventory Counts</h2>
      <p class="text" v-if="inventory > 10">
        We have inventory {{ inventory }} items in stock
      </p>
      <p class="text" v-else>Hurry, we are running Low</p>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        inventory: 3,
      };
    },
  };
  </script>
  
  <style scoped>
  body{
    width: 100%;
  }

  .inventory-container{
    background: aliceblue;
    padding: 20px;
    display: flex;
    align-items: center;
    margin: 0 auto;
    border-top: 1px solid silver;
    text-align: center;
    flex-direction: column;
    position: relative;
    width: 100%;
   
  }

  h2{
    text-align: center;
    margin: 0 auto;
    padding: 14px;
    color: #333;
    font-size: 2rem;
    font-weight: bold;
  }

  .text{
    background: darkslategray;
    width: 50%;
    margin: 0 auto;
    color: #fff;
    font-size: 1rem;
    text-align: center;
    padding: 12px;
    position: relative;
  }
  </style>
  