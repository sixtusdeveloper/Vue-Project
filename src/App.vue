<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Sixtus's First Vue project."/>
  <AltSchoolStudent />
  <FormInput />
  <ProductsItems />
  <InventoryCount />
  <SubmitForm />
  <StudentInputs />
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import AltSchoolStudent from './components/AltshoolStudent.vue'
import FormInput from './components/FormInput.vue'
import ProductsItems from './components/ProductItems.vue'
import InventoryCount from './components/InventoryCount.vue'
import SubmitForm from './components/SubmitForm.vue'
import StudentInputs from './components/StudentInput.vue'

// import { is } from 'core-js/fn/object'
// import { beforeCreate } from 'core-js/fn/object'



export default {
  name: 'App',
  components: {
    HelloWorld,
    AltSchoolStudent,
    FormInput,
    ProductsItems,
    InventoryCount,
    SubmitForm,
    StudentInputs
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
