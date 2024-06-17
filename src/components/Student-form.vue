<template>
    <div class="container">
        <h2>Name Verification Test</h2>
        <p>What is your name?</p>
        <p>{{ username }}</p>
        <button @click="handleSubmit">Submit</button>
        <!-- Your HTML code goes here -->
    </div>
</template>

<script>
export default {
    name: 'StudentForm',
    data() {
        return {
            // Your data properties go here
            username: 'Sixtusdev',
        };
    },
    methods: {
        // Your methods go here
        handleSubmit() {
            alert('You have submitted the form');
        },
    },

    handleKeyDown(event) {
        if (event.key === 'Enter') {
            this.handleSubmit();
            console.log('Enter key pressed');
        }
    },

    mounted() {
        // Code to run when the component is mounted goes here
        console.log('mounted has been invoked');

    },
};
</script>

<style scoped>
/* Your component-specific styles go here */
.container {
    margin: 0 auto;
    padding: 20px;
    width: 100%;
    border-top: 1px solid silver;
    background-color: #fff;
    border-radius: 5px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}

h2{
    text-align:center;
    margin: 0 auto;
    padding: 14px;
    color: #333;
    font-size: 2rem;
    font-weight: bold;

}
button{
    background-color: #4CAF50;
    padding: 10px 24px;
    border:none;
    outline: none;
    margin: 2rem auto;
    text-align:center;
    color: #f4f4f4;
    font-size: 1rem;
    font-weight: normal;
    cursor: pointer;
    border-radius: 5px;
}
button:hover {
    background-color: #45a049;
}
</style>