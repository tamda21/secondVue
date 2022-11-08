<template>
  <div>
  <form-helpers>
    <h2 slot="title">{{title}}</h2>
    <p slot="text">This is Paragraph Form</p>
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
      title:"This is Title Form"
    }
  }
}
</script>

<style>

</style>
