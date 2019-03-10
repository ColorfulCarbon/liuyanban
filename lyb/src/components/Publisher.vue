<template>
 <div>
  <input type="text">
  <button @click="tijiao()">提交</button>
 </div>
</template>
<script>
export default {
 methods: {
  tijiao(){
   console.log(123);
   }
 },
  
}
</script>
<style>
  input{
    color:red;
  }
</style>