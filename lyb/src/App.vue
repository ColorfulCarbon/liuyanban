<template>
  <div id="app">
    
   <li v-for="(item, index) in items">

   <Comment :comment-text="item.message" />
  </li>
    <Publisher />
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import Publisher from './components/Publisher.vue'
import Comment from './components/Comment.vue'
export default {
  name: 'app',
  data(){
    return {
      items: [
        { message: '123' },
        { message: '345' }
      ]
    }
  },
  components: {
    HelloWorld,
    Publisher,
    Comment

  },
  created() {
    
  },
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
