<template>
    <div>
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
    background-color: #000;
    color: #fff;
    text-align :center ;
    padding: 10px;
    
  }
</style>