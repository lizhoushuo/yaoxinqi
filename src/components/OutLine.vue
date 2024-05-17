<template>
  <div class="outline">
    <div class="top"><img src="../assets/imgs/容器 47@3x.png" alt="" class="img1" /> 百香果基地概要</div>
    <div class="tab">
      <div>
        <div class="imgs">
          <img src="../assets/imgs/组 3030@3x.png" alt="" />
          <div class="desc">
            <p>种植基地</p>
            <p style="color: #777033"><font>729</font>m²</p>
          </div>
        </div>
      </div>
      <div>
        <div class="imgs">
          <img src="../assets/imgs/组 3030@3x(1).png" alt="" />
          <div class="desc">
            <p>种植人数</p>
            <p><font>52</font>人</p>
          </div>
        </div>
      </div>
      <div>
        <div class="imgs">
          <img src="../assets/imgs/组 3030@3x(2).png" alt="" />
          <div class="desc">
            <p>地块数量</p>
            <p><font>36</font>个</p>
          </div>
        </div>
      </div>
    </div>
    <div>
      <div class="left">
        <p>监听设备</p>
        <p style="color: #777033">729</p>
      </div>
      <div class="right">
        <div v-for="item in list" :key="item.id">
          <p>{{ item.name }}</p>
          <p style="color: #fff">{{ item.num }}</p>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      list: [
        { name: "光感加测灯", num: 1, id: 1 },
        { name: "视频摄像头", num: 2, id: 2 },
        { name: "孢子检测仪", num: 7, id: 3 },
        { name: "环境传感器", num: 4, id: 4 }
      ]
    }
  }
}
</script>
<style lang="scss" scoped>
.outline {
  width: 100%;
  height: 100%;
  display: grid;
  grid-template:
    "a a a a a  " 1fr
    "b b b b b  " 1fr
    "b b b b b  " 1fr
    "c c c c c  " 1fr
    "c c c c c  " 1fr
    "c c c c c  " 1fr
    /1fr 1fr 1fr 1fr 1fr;
}
.outline div:nth-of-type(1) {
  grid-area: a;
  //  border-bottom:1px solid #ccc;
  display: flex;
  align-items: center;
  .img1 {
    width: 20px;
    height: 20px;
    margin: 0 10px;
  }
}
.outline div:nth-of-type(2) {
  grid-area: b;
}
.top {
  border-bottom: 1px solid #478671;
}
.tab {
  width: 100%;
  height: 100%;
  display: flex;
  justify-content: space-around;
  align-items: center;
  div {
    .desc {
      font-size: 12px;
    }
    img {
      width: 40px;
      height: 40px;
    }
  }
}
.outline div:nth-of-type(3) {
  grid-area: c;
  display: flex;
  justify-content: center;
  align-items: center;
  .left {
    width: 50%;
    height: 100%;
    display: flex;
    padding-top: 15px;
    font-size: 12px;
    flex-direction: column;
    // justify-content: center;
    background-image: url("../assets/imgs/Group 625@3x.png");
    background-repeat: no-repeat;
    background-size: cover;
    background-position: top;
  }
  .right {
    width: 50%;
    height: 100%;
    display: flex;
    flex-wrap: wrap;
    div {
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      font-size: 12px;
      width: 50%;
      height: 50%;
    }
  }
}
.outline div:nth-of-type(4) {
  grid-area: d;
}
.imgs {
  img {
    vertical-align: middle;
  }
}
</style>
