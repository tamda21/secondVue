<template>
  <div class="container">
    
<!-- 
  <form-helpers>
    <div slot='form-header'>
      <h3>This Title of Form</h3>
      <p>Information Of Form</p>
    </div>
    <div slot='form-feilds'>
      <input type="text" placeholder="username" required>
      <input type="password" placeholder="password" required>
    </div>
    <div slot='form-controls'>
      <button v-on:click="handelClick">Submit</button>
    </div>
  </form-helpers>
-->
  <keep-alive>
    <component v-bind:is="component"></component>
  </keep-alive>
    <a class="waves-effect waves-light btn-large" v-on:click="component='form-one'">Form One</a>
    <a class="waves-effect waves-light btn-large" v-on:click="component='form-two'">Form Two</a>
  </div>
    
</template>

<script>
//import FormHelpers from './Components/FormHelpers';
import FormOne from './Components/FormOne';
import FormTwo from './Components/FormTwo';
export default {
  components:{
   // 'form-helpers':FormHelpers
   'form-one':FormOne,
    'form-two':FormTwo
  },
  data () {
    return {
      component:'form-one'
    }
  }
}
</script>

<style>
/*#form-header{
  background-color: #eee;
  padding: 10px;
  margin: 20px auto;
}
#form-controls{
  background-color: #eee;
  padding: 10px;
  margin: 20px auto;
  text-align: center;
}
#form-controls button{
  padding: 10px;
  border: none;
  text-transform: uppercase;
  color: #f00;
  background-color: #333;
  border-radius: 5px;
}
#form-header h3{
  text-align: center;
  text-transform: capitalize;
  
}
#form-header p{
  text-align: center;
}

#form-feilds{
  background-color: #eee;
  padding: 10px;
  margin: 20px auto;
  text-align: center;
}
#form-feilds input{
  border: none;
  padding:20px;
  border-radius: 5px;
  background-color: #333;
  color: #fff;
  outline: none;
}
*/
</style>
