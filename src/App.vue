<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Sixtus's First Vue project."/>
  <AltSchoolStudent />
  <FormInput />
  <ProductsItems />
  <InventoryCount />
  <SubmitForm />
  <!-- <StudentInputs /> -->
</template>

<script>
import HelloWorld from './components/Hello-world.vue'
import AltSchoolStudent from './components/AltSchool-student.vue'
import FormInput from './components/Form-input.vue'
import ProductsItems from './components/Product-items.vue'
import InventoryCount from './components/Inventory-count.vue'
import SubmitForm from './components/Submit-form.vue'
// import StudentInputs from './components/StudentInput.vue'

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
