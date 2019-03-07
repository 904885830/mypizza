<template>
  <div id="app" class="container">
    <!-- 导航栏展示 -->
    <Header />
    
    
    <!-- 展示路由页面 -->
    <router-view/>
    <router-view name="history"></router-view>
    <router-view name="history"></router-view>


  </div>
</template>

<script>
import Header from '@/components/Header';
export default {
  name: 'App',
  data(){
    return{
      img:'./assets/logo.png'
    }
  },
  components:{
    'Header':Header
  }
}
</script>

<style>
/* #app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
} */
</style>
