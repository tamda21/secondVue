<template>
  <div>
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
  </div>
    
</template>

<script>
import FormHelpers from './Components/FormHelpers';
export default {
  components:{
    'form-helpers':FormHelpers
  },
  data () {
    return {
      
    }
  }
}
</script>

<style>

</style>
