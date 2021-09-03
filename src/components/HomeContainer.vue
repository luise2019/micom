<template>
  <div class="home--container">
    <div>
      <div class="main-bar">
        <div class="main-banner">
          <a href="http://"><img src="../assets/main-banner.jpg" alt="" srcset="" /></a>
        </div>
        <div class="aside-bar">
          <ul class="aside-list">
            <li class="side-item">
              <a href="http://">手机<span class="fa fa-angle-right"></span></a>
            </li>
            <li class="side-item">
              <a href="http://">电视<span class="fa fa-angle-right"></span></a>
            </li>
            <li class="side-item">
              <a href="http://">笔记本&nbsp;平板<span class="fa fa-angle-right"></span></a>
            </li>
            <li class="side-item">
              <a href="http://">家电<span class="fa fa-angle-right"></span></a>
            </li>
            <li class="side-item">
              <a href="http://">出行&nbsp;穿戴<span class="fa fa-angle-right"></span></a>
            </li>
            <li class="side-item">
              <a href="http://">智能&nbsp;路由器<span class="fa fa-angle-right"></span></a>
            </li>
            <li class="side-item">
              <a href="http://">电源&nbsp;配件<span class="fa fa-angle-right"></span></a>
            </li>
            <li class="side-item">
              <a href="http://">健康&nbsp;儿童<span class="fa fa-angle-right"></span></a>
            </li>
            <li class="side-item">
              <a href="http://">耳机&nbsp;音箱<span class="fa fa-angle-right"></span></a>
            </li>
            <li class="side-item">
              <a href="http://">生活&nbsp;箱包<span class="fa fa-angle-right"></span></a>
            </li>
          </ul>
        </div>
      </div>
      <div class="shortcut">
        <div class="short-ser">
          <ul class="ser-list">
            <li class="list-item"><a href="http://"><span class="fa fa-clock-o"></span>保障服务</a></li>
            <li class="list-item"><a href="http://"><span class="fa fa-clock-o"></span>保障服务</a></li>
            <li class="list-item"><a href="http://"><span class="fa fa-clock-o"></span>保障服务</a></li>
            <li class="list-item"><a href="http://"><span class="fa fa-clock-o"></span>保障服务</a></li>
            <li class="list-item"><a href="http://"><span class="fa fa-clock-o"></span>保障服务</a></li>
            <li class="list-item"><a href="http://"><span class="fa fa-clock-o"></span>保障服务</a></li>
          </ul>
        </div>
        <div class="photo">
          <ul class="photo-list">
            <li class="photo-item"><img src="../assets/9f18ac756fa2cedb16ea429b9c0001af.png" alt="" /></li>
            <li class="photo-item"><img src="../assets/b30177d629bfbe2fb42251c1b8538f7b.jpg" alt="" /></li>
            <li class="photo-item"><img src="../assets/d8a6d6d37904e22c72130e3e4ec79b41.jpg" alt="" /></li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "HomeContainer",
  props: {},
};
</script>

<style >
.home--container {
  height: 635px;
  padding-right: auto;
  padding-left: auto;
  display: flex;
  justify-content: center;
}
/* 主图容器设置 */
.main-bar{
  width: 1226px;
  height: 460px;
  position: relative;
}
.main-banner img{
  width: 100%;
}
/* 设置侧导航容器的尺寸和背景 ,相对容器绝对定位*/
.aside-bar{
  width:234px;
  height: 460px;
  padding-top: 20px;
  padding-bottom: 20px;
  background-color:rgba(105,101,101,.6);
  font-size: 14px;
  position: absolute;
  top: 0px;
  left: 0px;
  opacity: .7;
}
/* 设置侧导航的flex布局 */
.aside-list{
  display:flex;
  flex-flow: column wrap;
  justify-content:center;
  align-content: center;

}
/* 设置导航类目的尺寸和文字效果 */
.side-item{
  width: 234px;
  height: 42px;
  line-height: 42px;
  text-align: left;
  flex: 1 1 auto;
  padding-left: 30px;
}
/* 设置导航链接的效果 */
.aside-list .side-item a {
  width: 100%;
  color: #ffffff;
  display: inline-block;
}
/* 设置箭头浮动和居中，调整位置 */
.side-item a span{
  float:right;
  line-height: 42px;
  font-size: 20px;
  padding-right: 30px;
}
/* 设置鼠标移入变色 */
.side-item:hover{
  background-color: orange;
}
/* 设置shortcut容器 */
.shortcut{
  width: 100%;
  display: flex;
  margin-top:5px;
  margin-left: auto;
  margin-right: auto;

}
/* 设置short-ser的尺寸和背景 */
.short-ser{
  width: 234px;
  height: 170px;
  background-color: #5f5750;
  font-size: 12px;
  color: #ffffff;
}
/* 设置ser-list布局*/
.ser-list{
  display: flex;
  flex-flow: row wrap;
}
/* 设置list-item的尺寸和文字效果 */
.list-item{
  flex: 1 1 auto;
  width: 78px;
  height: 85px;
  line-height: 85px;
  text-align: center;
  border: 1px solid white;
}
/* 设置list-item的效果 */
.list-item  a {
  width: 100%;
  padding-top: 18px;
  color: #ffffff;
  display: inline-block;
  opacity: .7;
}
/* 设置图标效果 */
.list-item span{
  font-size: 25px;
}

/* 设置photo的尺寸和背景 */
.photo-list{
  display: flex;
  justify-content: flex-start;
}
/* photo-item的尺寸 */
.photo-item{
  width:321px;
  height: 170px;
  margin-left:10px;
}
.photo-item img{
  width: 100%;
}
</style>
