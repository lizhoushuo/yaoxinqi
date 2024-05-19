<template>
  <div class="Passion-box">
    <!-- 头部标题 -->
    <header>
      <div class="head-img">
        <img src="../../assets/imgs/容器 47@3x.png" alt="" />
      </div>
      <div class="head-title">
        <span>百香果基地预警</span>
      </div>
    </header>
    <!-- 主体部分 -->
    <section>
      <div class="section-box">
        <div class="section-image">
          <img src="../../assets/imgs/组 3299@2x.png" alt="" />
          <span>729</span>
        </div>
        <p>本周预222警数</p>
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
        <p>本周预警222数</p>
      </div>
    </section>
    <!-- 尾部 -->
    <footer>
      <!-- 尾部的按钮 -->
      <div class="time-button">
        <img src="../../assets/imgs/Rectangle 605@2x.png" alt="" />
        <span>小刘大帅哥</span>
      </div>

      <div class="center">
        <p>
          <span>小刘大帅哥</span>
          <span>223</span>
        </p>
        <p>
          <span>小刘大帅</span>
          <span>2323</span>
        </p>
      </div>

      <div class="right">
        <p>
          <span>小刘大帅</span>
          <span>21</span>
        </p>
        <p>
          <span>小刘大帅</span>
          <span>21</span>
        </p>
      </div>
    </footer>
  </div>
</template>

<style lang="scss">
.Passion-box {
  width: 100%;
  height: 100%;
  background-color: #317f786f;
  box-shadow: inset 1px 1px 20px #11211c;
  border-radius: 0.625rem;
}
.Passion-box > header {
  width: 100%;
  height: 25%;
  display: flex;
  align-items: center;
  border-bottom: 0.0625rem solid #317f786f;
  padding: 0 0 0 15px;
  .head-img {
    width: 4%;
    display: flex;
    align-items: center;
    margin-right: 2%;
    img {
      width: 100%;
    }
  }
  .head-title {
    width: 92%;
  }
}
section {
  width: 100%;
  // height: 49%;
  display: flex;
  align-items: center;
  // justify-content: space-around;
  border-bottom: 1px solid #317f786f;
}
section .section-box {
  display: flex;
  flex-direction: column;
  align-items: center;
  width: 33.3%;
  // text-align: center;
  p {
    // margin-top: 5px;
    color: #fff;
    font-size: 12px;
  }
}

// 把文字定位到图片中间
section .section-box .section-image {
  width: 55px;
  height: 55px;
  // height: 90px;?
  text-align: center;
  position: relative;
}
section .section-box .section-image img {
  width: 100%;
  height: 100%;
  // margin: auto;
}
section .section-box .section-image span {
  // font-size: 20px;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -99%);
  text-align: center;
}

// 改变每个文字的颜色
section .section-box:nth-child(1):nth-child(1) .section-image span {
  font-size: 0.75rem !important;
  color: red;
}
section .section-box:nth-child(2):nth-child(2) .section-image span {
  font-size: 0.75rem !important;
  color: #34645b;
}
section .section-box:nth-child(3):nth-child(3) .section-image span {
  font-size: 0.75rem !important;
  color: #7b7b33;
}

// 尾部
footer {
  width: 100%;
  height: 28%;
  font-size: 12px;
  display: flex;
  align-items: center;
  justify-content: space-around;
}

footer .time-button {
  width: 29.3%;
  height: 100%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  position: relative;
}
footer .time-button img {
  width: 70%;
  height: 30px;
  margin-left: 1.25rem;
  // line-height: 30px;
}
footer .time-button span {
  font-size: 12px;
  width: 100%;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  text-align: center;
  color: #843937;
}

.center {
  width: 33.3%;
  display: flex;
  flex-direction: column;
  p:nth-child(1) {
    display: flex;
  }
  p:nth-child(2) {
    display: flex;
    // color: black;
  }
  p:nth-child(1) span:nth-child(2) {
    color: #b93230;
  }
  p:nth-child(2) span:nth-child(2) {
    color: #b93230;
  }

  p:nth-child(1) span:nth-child(1) {
    // color: skyblue;
    width: 80px;
    display: block;
    margin-right: 5px;
    text-align: right;
  }
  p:nth-child(2) span:nth-child(1) {
    // color: blue;
    width: 80px;
    display: block;
    text-align: right;
    margin-right: 0.3125rem;
  }
}

.right {
  width: 33.3%;
  display: flex;
  flex-direction: column;
  p:nth-child(1) {
    display: flex;
  }
  p:nth-child(2) {
    display: flex;
    // color: black;
  }
  p:nth-child(1) span:nth-child(2) {
    color: #b93230;
  }
  p:nth-child(2) span:nth-child(2) {
    color: #b93230;
  }
  p:nth-child(1) span:nth-child(1) {
    // color: skyblue;
    width: 80px;
    display: block;
    margin-right: 5px;
    text-align: right;
  }
  p:nth-child(2) span:nth-child(1) {
    // color: blue;
    width: 80px;
    display: block;
    text-align: right;
    margin-right: 5px;
  }
}
</style>
