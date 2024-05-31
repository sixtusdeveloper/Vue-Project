<template>
    <div>
        <p v-for="Student in Students key:=`student.id`">{{ Student.name }}</p>
    </div>
</template>

<script>
export default {
    name: 'Student',
    data() {
        return {
            // In Array of Objects, each object has a unique id
            Student[
                {id: 1, name: 'John Doe', grade: 'A'},
                {id: 2, name: 'Jane Doe', grade: 'B'},
                {id: 3, name: 'John Smith', grade: 'C'},
                {id: 4, name: 'Jane Smith', grade: 'D'},
            ],
            
        };
    },
    computed: {
        Students() {
            return this.Student;
        },
    },
};
</script>

<style scoped>
body{
    background-color: #f0f0f0;
    text-align: center;
    margin: 0 auto;
}
</style>