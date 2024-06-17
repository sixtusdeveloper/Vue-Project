<template>
  <div class="hello">
    <div class="container">
    <h1>{{ msg }}</h1>
    <h3>AltSchool Students Incremental Game!</h3>
     <p>Hello Altshool students.</p>
     <p class="count-btn">{{ count }}</p>
     <button @click="incrementCount">Increment</button>
    </div>
  </div>
</template>

<script>
// import { is } from 'core-js/core/object';

// The script tag is where the logic of the component is defined.

// The export default statement is used to export a single default object, function, or primitive from a script file.
export default {
  name: 'HelloWorld',
  props: {
    msg: String,
  },


  // Data is a function that returns an object. This object contains the data that the component will use.
data() {
  return {
    count: 1
  }},


  // Mounted is a lifecycle hook that is called after the instance has been mounted.
  // mounted() {
  //   this.count += 20
  // },


  // Methods is an object that contains methods that are called when the instance is created.
 methods: {
    incrementCount() {
      this.count++;
    },
  },


  // BeforeCreate method is called before the instance is created. It is called before the created method.
   beforeCreate() {
    console.log('beforeCreate has been called');
  },
  
  // The Created mothod is called after the instance is created. It is called after the beforeCreate method.
  created() {
    console.log('Created has been called');
  },


  // BeforeMount method is called before the instance is mounted. It is called before the mounted method.
  beforeMount() {
    console.log('beforeMount has been called');
  },  


  // Mounted is a lifecycle hook that is called after the instance has been mounted.
  mounted() {
    console.log('mounted has been called');
  },


  // Before update method is called before the instance is updated. It is called before the updated method.
  beforeUpdate() {
    console.log('beforeUpdate has been called');
  },

  // Updated method is called after the instance is updated. It is called after the beforeUpdate method.
  updated() {
    console.log('updated has been called');
  },
}


</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
body{
  width: 100%;

}
.container{
  width: 100%;
  display: flex;
  flex-direction: column;
  margin: 0 auto;
  padding: 20px;
  background: aliceblue;


}
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
button{
padding: 10px 24px;
border: 1px solid #42b983;
outline: none;
background: transparent;
margin: 2rem auto;
text-align:center;
color: #333;
font-size: 1rem;
font-weight: normal;
cursor: pointer;
border-radius: 5px;

}
.count-btn{
  font-family: Georgia, 'Times New Roman', Times, serif;
  display: flex;
  justify-content: center;
  align-items: center;
  background: darkslategray;
  color: #ffff;
  font-size: 2rem;
  padding: 18px;
  border-radius: 5px;
  margin: 10px auto;
  text-align: center;
 width: 35px;
 position: relative;
}
</style>


