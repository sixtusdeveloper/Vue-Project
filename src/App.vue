<template>
  <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
  <HelloWorld msg="Welcome to Sixtus's Vue projects!"/>
  <AltSchoolStudent />
  <FormInput />
  <StudentForm />
  <GreetLogic />
  <StudentGrade />

  <!-- <StudentInputs /> -->
</template>

<script>
import HelloWorld from './components/Hello-world.vue';
import AltSchoolStudent from './components/AltSchool-student.vue';
import FormInput from './components/Form-input.vue';
import StudentForm from './components/Student-form.vue';
import GreetLogic from './components/GreetLogic.vue';
import StudentGrade from  './components/Student-Grade.vue';




export default {
  name: 'App',
  components: {
    HelloWorld,
    AltSchoolStudent,
    FormInput,  
    StudentForm,
    GreetLogic,
    StudentGrade,
  }
}

</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  overflow: hidden;
}
</style>
