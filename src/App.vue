<template>
  <h1>Hello Vue</h1>
  <span>{{ new Date().getDate() }}</span>
  <H6>Hi {{ first_name }}</H6>
  <h5>Age: {{ age + deathAge }}</h5>
  <button @click="getFullName">Get Full Name</button>
</template>

<!--Script API Method Start-->
<script setup>

let first_name = 'Bill'
let last_name = 'Gates'
let age = 65
let deathAge = 23
const getFullName = () => {
  alert('Bill Gates')
}

//Composition API Method Start

/* export default {
  setup() {
    let first_name = 'Bill'
    let last_name = 'Gates'
    let age = 65
    let deathAge = 23
    const getFullName = () => {
      alert('Bill Gates')
    }

    return { first_name, last_name, age, deathAge, getFullName }
  }

  // option API method Start

   data() {
     return {
       first_name: "Bill",
       last_name: "Gates",
       age: 65,
       deathAge: 23,
       getFullName: () => {
         alert("Bill Gates")
       }
     }
   }

   // option API method End
} */

//Composition API Method End
</script>

<!--Script API Method End-->

<style scoped></style>
