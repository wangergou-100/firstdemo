<template>
  <div id="app">
    <el-container>
      <el-header id="headerBook"> 
        <Header/> 
      </el-header>
      <el-main id="mainBook">
        <div id="mainBookWrapper">
         <!-- <Main/>-->
          <router-view></router-view>
        </div>
      </el-main>
      <el-footer id="footerBook">
        <Footer/>
      </el-footer>
    </el-container>
  </div>
</template>

<script>
//1、 导入组件
//2、注册组件
//3、 使用组件
import Header from './components/Header.vue'
import Main from './components/Main.vue'
import Footer from './components/Footer.vue'
export default {
  name: "App",
  components: {
    Header,
    Main,
    Footer
  },
};
</script>

<style>
* {
  margin: 0;
  padding: 0;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  /* text-align: center; */
  color: #2c3e50;
  /* margin-top: 60px; */
  /* background-color: blue; */
  height: 100%;
}
#headerBook{
  background-color: #244152;
}
#mainBook{
  /* background-color: green; */
}
#footerBook{
  /*background-color:yellow;*/
}
#mainBookWrapper{
  height: 450px;
}
</style>
