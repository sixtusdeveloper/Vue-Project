<template>
    <div class="container">
        <h2>Grade Score calculator</h2>
        <!-- The component content goes here -->
         <p>What is Andres's second grade score?</p>
         <span>{{ getUserGrade }}</span>

    </div>
</template>

<script>
export default {
    // The component logic goes here
    data() {
        return {
            // The data properties go here
            Username: "",

            user: {
                name: 'Andre',

                grades: {
                    Primary: 'A',
                    Secondary: 'C', 
                    Tertiary: 'B'
                },
            },
        };
    },
    computed: {
        // The computed properties go here
        getUserGrade(){
            return this.user.grades.Secondary;
        },
    },

    methods: {
        userGrade(){
            return this.user.grades.Secondary;  
        },
    },
}
</script>

<style scoped>
/* The component styles go here */
.container {
    background: darkslategray;
        padding: 30px;
        display: flex;
        align-items: center;
        margin: 0 auto;
        border-top: 1px solid silver;
        text-align: center;
        flex-direction: column;
        position: relative;
        width: 100%;
        color: #fff;
}

h2{
    font-size: 2rem;
    font-weight: bold;
    color: #fff;
    text-align:center;
    margin: 0 auto;
    padding: 1.5rem;

}

span{
    background: transparent;
    margin: 0 auto;
    width: 50px;
    color: #fff;
    border: 1px solid #777;
    border-radius: 6px;
    font-size: 1rem;
    text-align: center;
    padding: 14px 20px;
    position: relative;
}





</style>