<template>
  <div id="app">
    <Header />
    <HomeContainer />
  </div>
</template>

<script>
import Header from './components/Header'
import HomeContainer from './components/HomeContainer'
export default {
  name: 'App',
  components: {
    Header,HomeContainer,
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
  font-family: "Helvetica Neue", Helvetica, Arial, "Microsoft Yahei", "Hiragino Sans GB", "Heiti SC", "WenQuanYi Micro Hei", sans-serif; box-sizing: border-box; } *{
  margin: 0px;
  padding: 0px;
  box-sizing: border-box;
}
body{
  min-width: 1226px;
}
.container{
  margin: 0 auto;
}
a{
  text-decoration: none;
}
ul{
  padding: 0;
  list-style: none;
}

.clearfix ::after{
  content: "";
  display: table;
  clear: both;
}
</style>
