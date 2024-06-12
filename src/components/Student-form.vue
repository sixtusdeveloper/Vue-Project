<template>
    <div class="container">
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
    width: 50%;
    background-color: #f0f0f0;
    border-radius: 5px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}
button{
    background-color: #4CAF50;
    color: white;
    padding: 10px 20px;
    margin: 10px 0;
    border: none;
    border-radius: 5px;
    cursor: pointer;
}
button:hover {
    background-color: #45a049;
}
</style>