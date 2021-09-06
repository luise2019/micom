<template>
  <div class="home--container">
    <div class="main-container">
    <div class="main-bar">
      <div class="main-banner">
        <a href="http://"><img src="../assets/main-banner.jpg" alt="" srcset="" /></a>
      </div>
      <div class="aside-bar">
        <ul class="aside-list">
          <li v-for="item in templatelist" :key="item" class="side-item">
          <a :href="item.link"><span :class="item.span"></span>{{ item.label }}</a>
        </li>
        </ul>
      </div>
    </div>
    <div class="shortcut">
      <div class="short-ser">
        <ul class="ser-list">
          <li v-for="item in shortcutlist" :key="item" class="list-item">
          <a :href="item.link"><span :class="item.span"></span>{{ item.label }}</a>
        </li>
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
    <div class="back-top">
      <span class="fa fa-mobile"></span>
      <span class="fa fa-user-o"></span>
      <span class="fa fa-wrench"></span>
      <span class="fa fa-headphones"></span>
      <span class="fa fa-shopping-cart"></span>
    </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "HomeContainer",
  props: {},
  data() {
    return {
      templatelist:[
        {label:"手机",link: "#",span:"fa fa-angle-right"},
        {label:"电视",link: "#",span:"fa fa-angle-right"},
        {label:"笔记本 平板",link: "#",span:"fa fa-angle-right"},
        {label:"家电",link: "#",span:"fa fa-angle-right"},
        {label:"出行 穿戴",link: "#",span:"fa fa-angle-right"},
        {label:"智能 路由器",link: "#",span:"fa fa-angle-right"},
        {label:"电源 配件",link: "#",span:"fa fa-angle-right"},
        {label:"健康 儿童",link: "#",span:"fa fa-angle-right"},
        {label:"耳机 音箱",link: "#",span:"fa fa-angle-right"},
        {label:"生活 箱包",link: "#",span:"fa fa-angle-right"},
        ],
      shortcutlist:[
        {label:"小米秒杀",link: "#",span:"fa fa-clock-o"},
        {label:"企业团购",link: "#",span:"fa fa-clock-o"},
        {label:"F码通道",link: "#",span:"fa fa-clock-o"},
        {label:"米粉卡",link: "#",span:"fa fa-clock-o"},
        {label:"以旧换新",link: "#",span:"fa fa-clock-o"},
        {label:"话费充值",link: "#",span:"fa fa-clock-o"},
      ],
    };
  }
};
</script>

<style >
.home--container {
  height: 635px;
  
}
.main-container{
  display:flex;
  flex-direction: column;
  align-items: center;
}
/* 主图容器设置 */
.main-bar{
  width: 1226px;
  height: 460px;
  position: relative;
  flex: 1;
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
/* 设置侧导航的flex布局，垂直排列*/
.aside-list{
  display:flex;
  flex-flow: column wrap;
  /* justify-content:center;
  align-content: center; */
  
}
/* 设置导航类目的尺寸和文字效果 */
.side-item{
  width: 234px;
  height: 42px;
  line-height: 42px;
  text-align: left;
  flex: 1;
  
}
/* 设置导航链接的效果 */
.aside-list .side-item a {
  display: inline-block;
  width: 100%;
  color: #ffffff;
  padding-left: 30px;
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
  justify-content: center;
  margin-left: auto;
  margin-right: auto;

}
/* 设置short-ser的尺寸和背景 */
.short-ser{
  width: 234px;
  height: 170px;
  background-color: #5f5750;
  font-size: 12px;
  color: #cfccca;
}
/* 设置ser-list布局*/
.ser-list{
  display: flex;
  flex-flow: row wrap;
}
/* 设置list-item的尺寸和文字效果 
边框样式与实际有差，样式用绝对定位，伪元素插入每个li处理*/
.list-item{
  flex: 1 1 auto;
  width: 78px;
  height: 85px;
  border: 1px solid #cfccca;
}
/* 设置list-item内a元素的效果*/
.list-item  a {
  width: 100%;
  color: #cfccca;
  opacity: .7;
}
/* 设置图标效果 ,水平居中,和文字拉开距离*/
.list-item span{
  display: block;
  font-size: 35px;
  margin-top: 10px;
  margin-bottom: 10px;

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
  overflow: hidden;
}
/* 设置图片宽度继承父元素宽度，但画面有超出，父元素设置overflow解决 */
.photo-item img{
  width: 100%;
}

/*设置backtop样式 ,固定定位，窗口的右侧*/
.back-top{
  display: flex;
  flex-direction: column;
  width: 30px;
  position: fixed;
  bottom: 60px;
  right: 0;
  /*以下实现置紧贴容器的backtop
  right:50%;
  margin-right: -639px; */
  border-bottom-color: rgba(105,101,101,.6);
}
/* 设置backtop 图标样式 */
.back-top span{
  width: 30px;
  height: 30px;
  font-size: 30px;
  padding-top:10px;
  margin: 0 auto 8px;
}

</style>
