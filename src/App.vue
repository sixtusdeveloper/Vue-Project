<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Sixtus's First Vue project."/>
  <AltSchoolStudent />
  <FormInput />

  <!-- <StudentInputs /> -->
</template>

<script>
import HelloWorld from './components/Hello-world.vue'
import AltSchoolStudent from './components/AltSchool-student.vue'
import FormInput from './components/Form-input.vue'

// import { is } from 'core-js/fn/object'
// import { beforeCreate } from 'core-js/fn/object'



export default {
  name: 'App',
  components: {
    HelloWorld,
    AltSchoolStudent,
    FormInput,  
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
  margin-top: 60px;
}
</style>
