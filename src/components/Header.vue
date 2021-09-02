<template>
  <div class="container">
    <div class="topbar-wrapper">
      <ul class="TopBar">
        <li class="ser-items"><a href="">小米商城</a></li>
        <li class="spacer">|</li>
        <li class="ser-items"><a href="">MIUI</a></li>
        <li class="spacer">|</li>
        <li class="ser-items"><a href="">IoT</a></li>
        <li class="spacer">|</li>
        <li class="ser-items"><a href="">云服务</a></li>
        <li class="spacer">|</li>
        <li class="ser-items"><a href="">天星数科</a></li>
        <li class="spacer">|</li>
        <li class="ser-items"><a href="">有品</a></li>
        <li class="spacer">|</li>
        <li class="ser-items"><a href="">小爱开放平台</a></li>
        <li class="spacer">|</li>
        <li class="ser-items"><a href="">企业团购</a></li>
        <li class="spacer">|</li>
        <li class="ser-items"><a href="">资质证照</a></li>
        <li class="spacer">|</li>
        <li class="ser-items"><a href="">协议规则</a></li>
        <li class="spacer">|</li>
        <li class="ser-items"><a href="">下载app</a></li>
        <li class="spacer">|</li>
        <li class="ser-items"><a href="">智能生活</a></li>
        <li class="spacer">|</li>
        <li class="ser-items"><a href="">Select Location</a></li>
      </ul>
    <div class="shop-cart">
      <span class="fa fa-shopping-cart"></span>
      <a href="">购物车<span>(0)</span></a>
    </div>
    <ul class="personal-list">
        <li class="personal-items"><a href="">登入</a></li>
        <li class="spacer">|</li>
        <li class="personal-items"><a href="">注册</a></li>
        <li class="spacer">|</li>
        <li class="personal-items"><a href="">消息通知</a></li>
      </ul>
    </div>
    <div class="header-wrapper">
      <a href="" class="logo"><img src="../assets/logo-mi2.png" alt=""></a>
        <ul class="nav-list">
          <li class="nav-items"><a href="http://" >小米手机</a></li>
          <li class="nav-items"><a href="http://" >Redmi红米</a></li>
          <li class="nav-items"><a href="http://" >电视</a></li>
          <li class="nav-items"><a href="http://" >笔记本</a></li>
          <li class="nav-items"><a href="http://" >平板</a></li>
          <li class="nav-items"><a href="http://" >家电</a></li>
          <li class="nav-items"><a href="http://" >路由器</a></li>
          <li class="nav-items"><a href="http://" >智能硬件</a></li>
          <li class="nav-items"><a href="http://" >服务</a></li>
          <li class="nav-items"><a href="http://" >社区</a></li>
        </ul>
      <div class="searchbox">
        <div class="input"></div>
        <span class="fa fa-search"></span>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Header',
  props: {
    
  }
}
</script>

<style>
.container{
  height: 140px;
  top:0px;
  left:0px;

}
.topbar-wrapper{
  min-width: 1226px;
  height: 40px;
  line-height: 40px;
  background-color: #333;
  font-size: 12px;
  color: #b0b0b0;
  margin-left: auto;
  margin-right: auto;
}
.ser-items,.spacer,.personal-items,.logo,.nav-items {
  float: left;
}
.shop-cart,.personal-list,.searchbox {
  float: right;
}
.TopBar{
  height:40px;
}
.topbar-wrapper a{
  color: #b0b0b0;
}
.shop-cart {
  width: 120px;
  height: 40px;
  text-align: center;
  margin-left: 15px;
}
.header-wrapper{
  width: 100%;
  height: 100px;
  line-height: 100px;
  font-size: 16px;
  }
.logo{
  width: 62px;
  height: 56px;
  margin-top: 22px;
}
.header-wrapper .nav-list{
  width:850px;

}
.nav-list a{
  color: rgb(0, 0, 0);
}

.spacer{
  margin: 0 0.3em;
  overflow: hidden;
  color:#424242;
}
img{
  width: 100%;
}
</style>