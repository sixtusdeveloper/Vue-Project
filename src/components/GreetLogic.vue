<template>
    <div class="container">
        <h2>Greeting Print Out text</h2>
        <!-- Your template code goes here -->
         <button v-on:click="greet">Greeting</button>
    </div>
</template>

<script>
export default {
    data() {
        return {
            // Your data properties go here
            name: 'Sixtusdev',
            
        }
    },
    // Your script code goes here
    methods: {
        greet(event) {
            if(event){
                console.log(event.target.tagName);
            }
            alert(`Hello ${this.name}! `)
        }
    }

}
</script>

<style scoped>
    /* Your component styles go here */
    .container{
        background: aliceblue;
        padding: 20px;
        display: flex;
        align-items: center;
        margin: 1rem auto;
        text-align: center;
        flex-direction: column;
        position: relative;
        width: 100%;
    } 

    button{
        padding: 10px 24px;
        border:none;
        outline: none;
        background: #047aed;
        margin: 2rem auto;
        text-align:center;
        color: #f4f4f4;
        font-size: 1rem;
        font-weight: normal;
        cursor: pointer;
        border-radius: 5px;
        
    }
    h2{
        text-align: center;
        margin: 0 auto;
        padding: 14px;
        color: #333;
        font-size: 2rem;
        font-weight: bold;

    }
</style>