<template>
  <div class="Passion-box">
    <!-- 头部标题 -->
    <header>
      <img src="../../assets/imgs/容器 47@3x.png" alt="" />
      <span>百香果基地预警</span>
    </header>
    <!-- 主体部分 -->
    <section>
      <div class="section-box">
        <div class="section-image">
          <img src="../../assets/imgs/组 3299@2x.png" alt="" />
          <span>729</span>
        </div>
        <p>本周预警数</p>
      </div>
      <div class="section-box">
        <div class="section-image">
          <img src="../../assets/imgs/组 3300@2x.png" alt="" />
          <span>57</span>
        </div>
        <p>本周预警数</p>
      </div>
      <div class="section-box">
        <div class="section-image">
          <img src="../../assets/imgs/组 3301@2x.png" alt="" />
          <span>48%</span>
        </div>
        <p>本周预警数</p>
      </div>
    </section>
    <!-- 尾部 -->
    <footer>
      <!-- <div class="time">
        <img src="../../assets/imgs/Rectangle 605.png" alt="" />
        <span>小刘大帅哥</span>
      </div>
      <div class="center">
        <p><font style="">小刘大帅哥</font><font>29</font></p>
        <p><font>小刘大帅</font><font>17</font></p>
      </div>
      <div class="right">
        <p><font style="color: #fff; margin-right: 10px">小刘大帅</font><font>29</font></p>
        <p><font style="color: #fff; margin-right: 10px">小刘大帅</font><font>217</font></p>
      </div> -->
    </footer>
  </div>
</template>

<style lang="scss">
.Passion-box {
  width: 100%;
  height: 100%;
  background-color: #317f786f;
  box-shadow: inset 1px 1px 20px #11211c;
  border-radius: 10px;
}
.Passion-box > header {
  height: 25%;
  display: flex;
  align-items: center;
  border-bottom: 1px solid #317f786f;
  padding: 0 0 0 15px;

  img {
    width: 16px;
    margin-right: 8px;
  }
}
section {
  height: 47%;
  display: flex;
  align-items: center;
  // text-align: center;
  justify-content: space-around;
  border-bottom: 1px solid #317f786f;
}
section .section-box {
  // padding: 15px;

  p {
    // margin-top: 5px;
    color: #fff;
    font-size: 12px;
  }
}

// 把文字定位到图片中间
section .section-box .section-image {
  width: 50px;
  // height: 90px;?

  position: relative;
}
section .section-box .section-image img {
  width: 100%;
  margin: auto;
}
section .section-box .section-image span {
  // font-size: 20px;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -90%);
  text-align: center;
}

// 改变每个文字的颜色
section .section-box:nth-child(1):nth-child(1) .section-image span {
  font-size: 12px !important;
  color: red;
}
section .section-box:nth-child(2):nth-child(2) .section-image span {
  font-size: 12px !important;
  color: #34645b;
}
section .section-box:nth-child(3):nth-child(3) .section-image span {
  font-size: 12px !important;
  color: #7b7b33;
}

// 尾部
// footer {
//   width: 100%;
// 	height: 23%;

//   // height: 100px;
//   display: flex;
//   align-items: center;
//   justify-content: space-around;
// }
// footer .time {
//   width: 23.3%;
//   position: relative;
// }
// footer .time img {
//   width: 100%;
// }
// footer .time span {
//   width: 100%;
//   position: absolute;
//   top: 50%;
//   left: 50%;
//   transform: translate(-50%, -60%);
//   text-align: center;
//   color: #843937;
// }
// footer .center {
//   width: 33.3%;
//   text-align: center;
//   // border: 1px solid red;
// }
// footer .center p:nth-child(1) font:nth-child(1) {
// 	font-size: 14px;
//   margin-right: 10px;
//   color: #fff;
// }
// footer .center p:nth-child(2) font:nth-child(1) {
//   color: #fff;
//   margin-right: 10px;
// }
// footer .center p:nth-child(1) {
//   // color: red;
//   float: right;
// }
// footer .center p:nth-child(2) {
//   // color: red;
//   float: right;
// }
// footer .right {
//   // border: 1px solid red;
// }
</style>
