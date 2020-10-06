<template>
  <div id="app">
    <!-- App.vue根组件通常不做处理，放入router-view视图，嵌套加载其他的组件 -->
    <router-view></router-view>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
// import axios from 'axios'
// import jsonp from 'jsonp'
import storage from './storage'

export default {
  name: 'App',
  components: {
    // HelloWorld
  },
  data(){
    return{
      // age:30
    }
  },
  mounted(){
    // let url="/activity/servicetime";
    // jsonp(url,(err,res)=>{
    //   let result=res;
    //   this.data=result;
    // })
    // storage.setItem('a',1);
    // storage.setItem('user',{a:1});
    // storage.setItem('abc',{a:1},'user');
    // storage.clear('a');
    storage.clear('a','user');
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
