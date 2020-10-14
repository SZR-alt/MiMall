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
// import storage from './storage'

export default {
  name: 'app',
  components: {
    // HelloWorld
  },
  data(){
    return{
      // age:30
      // res:{}
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
    // storage.clear('a','user');

    // 本地加载请求静态json文件的形式
    // this.axios.get('/mock/user/login.json').then((res)=>{
    //   this.res=res;
    // });
    // 通过easy-mock平台实现数据mock
    // this.axios.get('/user/login').then((res)=>{
    //   this.res=res;
    // });
    // 本地集成mockjs实现数据mock
    // this.axios.get('/user/login').then((res)=>{
    //   this.res=res;
    // });
  }
}
</script>

<style lang="scss">
  @import './assets/scss/reset.scss';
  @import './assets/scss/config.scss';
  @import './assets/scss/button.scss';
</style>
