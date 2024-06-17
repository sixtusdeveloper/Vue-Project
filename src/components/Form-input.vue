<template>
    <div class="container">
        <h2>Enter your Username:</h2>
        <input v-model="username" />
        <button v-show="username" @click="submit">Login</button>
    </div>
</template>

<script>
export default {
    name: 'FormInput',
    data() {
        return {
           username : ''
        };
    },
    methods: {
        submit() {
            alert('You are logged in');
        },
    },
    computed: {
        isUsernameEmpty() {
            return this.username === '';
        },
    },
    mounted() {
        console.log('mounted has been invoked');
    },
};
</script>

<style scoped>
  body{
    width: 100%;
  }

  .container{
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
    font-size: 2rem;
    font-weight: bold;
    color: #333;
    padding: 10px;
    margin: 0 auto;
  }

  input{
    padding: 10px 20px;
    margin: 10px auto;
    width: 40%;
    position: relative;
    border: none;
    border-radius: 5px;
    outline: none;
    background: #ffffff;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
  }
  input:focus{
    border: 1px solid #047aed;
  }

  button{
    padding: 10px 20px;
    margin: 12px auto;
    border: none;
    border-radius: 5px;
    cursor: pointer;
    background: #047aed;
    color: #f4f4f4;
    font-size: 1rem;
    font-weight: normal;
    outline: none;
  }
</style>