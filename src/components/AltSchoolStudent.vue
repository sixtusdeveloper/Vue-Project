<template>
    <h1>{{ msg }}</h1>
    <div>
      <p v-if="inventory > 10">
        We have inventory {{ inventory }} items in stock
      </p>
      <p v-else>Hurry, we are running Low</p>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        inventory: 13,
      };
    },
  };
  </script>
  
  <style scoped>
  .read-the-docs {
    color: #888;
  }
  </style>
  