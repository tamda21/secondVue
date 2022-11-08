<template>
 <div>
     <h1>Please Fill Out Our Form...</h1>
     <form>
       <div id="form-header">
         <slot name='form-header'></slot>
       </div>
       <div id="form-feilds">
         <slot name='form-feilds'></slot>
       </div>
       <div id="form-controls">
         <slot name='form-controls'></slot>
       </div>
       <div id="form-links">
           <ul>
             <li><a href="#">link1</a></li>
             <li><a href="#">link2</a></li>
             <li><a href="#">link3</a></li>
             <li><a href="#">link4</a></li>
           </ul>
       </div>
     </form>
 </div>
</template>

<script>
export default {
    
  data () {
    return {
      
    }
  }
}
</script>

<style>
#form-links{
  background-color: #eee;
  padding: 20px;
  margin: 10px auto;
  text-align: center;
}
#form-links ul{
  padding: 0;
  list-style-type: none;
}
li{
  display: inline-block;
  margin-left: 8px
}
li:hover{
  background-color: #333;
  padding: 10px;
}
li:hover a{
  color: #f00;
  pointer-events: none;
}
li a{
  text-decoration: none;
  color: #333;
}
</style>
