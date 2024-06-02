<template>
  <div class="home">
 <p>  My name is    {{name}} and My age is  {{age}}</p>
 <button  @click="HandleClick"> Click Me</button>
 <button @click="age++">Add 1 to the  Age </button>
 <input v-model="name"> 
  </div>
</template>

<script>
import { ref } from 'vue';


export default {
  name: 'HomeView',
  setup(){
 
    const age = ref(35);
    const name= ref('mario')

    const HandleClick = () =>  {
     name.value='ahmed' ,

     age.value =3555
    }
    return {name , age,HandleClick}
  }

}
</script>
