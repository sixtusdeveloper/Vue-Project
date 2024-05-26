<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Sixtus's First Vue project."/>
  <AltSchoolStudent />
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import AltSchoolStudent from './components/altshool-student.vue'
export default {
  name: 'App',
  components: {
    HelloWorld,
    AltSchoolStudent
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
