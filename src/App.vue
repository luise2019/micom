<template>
  <div id="app">
    <Header />
  </div>
</template>

<script>
import Header from './components/Header'

export default {
  name: 'App',
  components: {
    Header,
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
  font-family: "Helvetica Neue", Helvetica, Arial, "Microsoft Yahei", "Hiragino Sans GB", "Heiti SC", "WenQuanYi Micro Hei", sans-serif;

}
*{
  margin: 0px;
  padding: 0px;
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
