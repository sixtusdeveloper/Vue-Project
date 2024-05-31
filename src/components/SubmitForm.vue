<template>
    <div>
        <button v:on:click="submit">Pay</button>
    </div>
</template>

<script>
export default {
    name: 'SubmitForm',
    data(){},
    methods:{
        submit(){
            console.log('Payment Successful');
        
        }
    },
};
</script>

<style scoped>
body {
    background-color: #f0f0f0;
    text-align: center;
    margin: 0 auto;
}
</style>