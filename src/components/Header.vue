<template>
  <div class="header--container">
    <div class="topbar-background">
      <div class="topbar-wrapper">
        <ul class="topbar--left">
          <li class="ser-items"><a href="">小米商城</a></li>
          <li class="spacer">&nbsp;|&nbsp;</li>
          <li class="ser-items"><a href="">MIUI</a></li>
          <li class="spacer">&nbsp;|&nbsp;</li>
          <li class="ser-items"><a href="">IoT</a></li>
          <li class="spacer">&nbsp;|&nbsp;</li>
          <li class="ser-items"><a href="">云服务</a></li>
          <li class="spacer">&nbsp;|&nbsp;</li>
          <li class="ser-items"><a href="">天星数科</a></li>
          <li class="spacer">&nbsp;|&nbsp;</li>
          <li class="ser-items"><a href="">有品</a></li>
          <li class="spacer">&nbsp;|&nbsp;</li>
          <li class="ser-items"><a href="">小爱开放平台</a></li>
          <li class="spacer">&nbsp;|&nbsp;</li>
          <li class="ser-items"><a href="">企业团购</a></li>
          <li class="spacer">&nbsp;|&nbsp;</li>
          <li class="ser-items"><a href="">资质证照</a></li>
          <li class="spacer">&nbsp;|&nbsp;</li>
          <li class="ser-items"><a href="">协议规则</a></li>
          <li class="spacer">&nbsp;|&nbsp;</li>
          <li class="ser-items download"><a href="">下载app<div class="box1"></div><span class="qrcode"><img src="../assets/download.png" alt="" >小米商城APP</span></a></li>
          <li class="spacer">&nbsp;|&nbsp;</li>
          <li class="ser-items"><a href="">智能生活</a></li>
          <li class="spacer">&nbsp;|&nbsp;</li>
          <li class="ser-items"><a href="">Select Location</a></li>
        </ul>
        <div class="topbar--right">
          <ul class="personal-list">
            <li class="personal-items"><a href="">登入</a></li>
            <li class="spacer">&nbsp;|&nbsp;</li>
            <li class="personal-items"><a href="">注册</a></li>
            <li class="spacer">&nbsp;|&nbsp;</li>
            <li class="personal-items"><a href="">消息通知</a></li>
          </ul>
          <div class="shop-cart">
              <a href=""><span class="fa fa-shopping-cart"></span>
             &nbsp;购物车<span>(0)</span></a>
             <div class="cart-menu">
               <div class="menu-content"></div>
             </div>
          </div>
          
        </div>
      </div>
    </div>
    <div class="header-wrapper">
        <a href="" class="logo"><img src="../assets/logo-mi2.png" alt=""></a>
        <ul class="nav-list">
          <li class="nav-items"><a href="http://" >小米手机</a>
          <!--  -->
          </li>
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
        
      <div class="header-search">
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
.header--container{
  height: 140px;
  top:0px;
  left:0px;
}

.topbar-background {
  height: 40px;
  line-height: 40px;
  background-color: #333;
  font-size: 12px;
  color: #b0b0b0;
}

.topbar-background a {
  color: #b0b0b0;
  display: block;
}

.topbar--left a:hover,.topbar--right a:hover{
  color: white;
}

.shop-cart:hover,.shop-cart a:hover{
  color: orange;
}

.topbar-wrapper {
  width: 1226px;
  margin-left: auto;
  margin-right: auto;
  display: flex;
  justify-content: space-between;
}
.topbar--left {
  height:40px;
}
/* 设置下拉菜单 */
.topbar--left .download,.topbar--right .shop-cart{
  position: relative;
  z-index: 99;
}
/* 设置菜单上的三角形 */
.download .box1{
  display: none;
  width: 0;
  height: 0;
  border: 8px solid #333;
  border-bottom-color: rgb(255, 255, 255);
  border-top:none;
  position:absolute;
  top: 32px;
  left:15px;
}
/* qrcode的下拉菜单 */
.download .qrcode{
  display: none; 
  width: 124px;
  height:148px;
  font-size: 14px;
  color: black;
  background-color: white;
  box-shadow: 0px 1px 5px #b0b0b0;
  text-align: center;
  /* 根据该元素本身的字体大小 设置行高，等于line-height 100% */
  line-height: 1;
  position:absolute;
  top: 40px;
  left:-39px;
  /* 对菜单添加动画效果 */
  transition: height .3s; 
  /* 添加z系数 */
  z-index: 10;
}
/* 设置hover显示 */
.download:hover .qrcode,.download:hover .box1{
  display: block;
}
/* 设置二维码居中 */
.qrcode img{
  width:90px;
  margin: 17px;
}
.topbar--right{
  width:263px;
}
/* 购物车的下拉菜单,实际还需有加载动画，商品列表，购物提示*/
.cart-menu{
  display: none;
  width: 316px;
  height: 100px;
  background-color: white;
  box-shadow: 0px 1px 5px #b0b0b0;
  position:absolute;
  top: 40px;
  left:-196px;
  /* 设置 */
  z-index: 10;
}
/* 购物车鼠标hover特效 */
.shop-cart:hover {
 background-color: white;
 border-bottom: none;
 padding-bottom:5px;
}
/* 设置hover显示 */
.shop-cart:hover .cart-menu{
  display: block;
}

/* 之后优化下只用flex实现布局 */
.ser-items,.spacer,.personal-items,.nav-items{
  float: left;
}
.shop-cart,.header-search {
  float: right;
}

.shop-cart {
  width: 120px;
  height: 40px;
  margin-left: 5px;
  background-color: #424242;
}
.header-wrapper{
  width: 100%;
  height: 100px;
  line-height: 100px;
  font-size: 16px;
  display: flex;
  justify-content: center;
  }
  
.logo{
  width: 62px;
  height: 56px;
  margin-top: 22px;
  margin-right: 50px;
}
/* 靠右边的导航条，靠近主轴end */
.header-wrapper .nav-list{
  width:810px;
  display: flex;
  justify-content: flex-end;
}
/* 子项平分容器，需要优化缩小空隙 */
.nav-list .nav-items{
  height: 88px;
  flex: 1 1 0;
}
.nav-list a{
  display: inline-block;
  color: rgb(0, 0, 0);
}

.nav-list a:hover{
  color: orange;
}

/* 设置nav-list的下拉菜单 待补*/
/* .child-container {
  width: 1226px;
} */

/* 搜索表单后续优化 ,此处用盒子假装一下*/
.header-search{
  width: 296px;
  display: flex;
  align-items: center;
  
}
.header-search .input{
  width: 80%;
  height: 48px;
  border:1px #b0b0b0 solid;
  /* 容器设置align-items或子项设置align-self: center;实现垂直居中 */
}
.header-search span{
  width: 20%;
  height: 48px;
  font-size: 30px;
  border:1px #b0b0b0 solid;
  padding: 6px;
}

.spacer{
  margin: 0 0.3em;
  color:#424242;
}
img{
  width: 100%;
}
</style>
