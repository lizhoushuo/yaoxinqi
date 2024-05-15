<template>
  <div class="dynamics">
    <div class="dynamics-top">
      <div><img src="../../assets/百香果数字运营中心/容器 47@2x.png" alt="" /><span>地块动态</span></div>
      <button>全部</button>
    </div>
    <div class="dynamics-content">
      <div>
        <div><img src="../../assets/百香果数字运营中心/组 239.png" alt="" /> <span>科研地块 &emsp; 台湾1号</span></div>
      </div>
      <div>
        <div>
          <button style="margin-right: 5px">详情</button><button style="margin-right: 5px">详情</button
          ><button>详情</button>
        </div>
      </div>
    </div>
    <div class="dynamics-content">
      <div>
        <div>
          <img src="../../assets/百香果数字运营中心/组 3030(2).png" alt="" /> <span>科研地块 &emsp; 台湾1号</span>
        </div>
      </div>
      <div>
        <div>
          <button style="margin-right: 5px">详情</button><button style="margin-right: 5px">详情</button
          ><button>详情</button>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {}
  },
  methods: {}
}
</script>
<style lang="scss" scoped>
.dynamics {
  width: 100%;
  height: 100%;
  .dynamics-top {
    width: 100%;
    height: 50px;
    display: flex;
    align-items: center;
    justify-content: space-between;
    border-bottom: 1px solid #fff;
    font-size: 13px;
    padding: 10px;
    box-sizing: border-box;
    color: #fff;
    img {
      margin-right: 10px;
      vertical-align: middle;
    }
    button {
      width: 60px;
      height: 30px;
      border-radius: 20px;
      font-size: 12px;
      background-color: rgb(25, 45, 37);
      border: #fff;
      color: #fff;
    }
  }
  .dynamics-content {
    padding: 10px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    div:nth-of-type(1) {
      color: #8aa96b;
      font-size: 13px;
      img {
        vertical-align: middle;
        margin-right: 10px;
        width: 25.59px;
        height: 25.59px;
      }
    }
    div:nth-of-type(2) {
      color: #8aa96b;
      font-size: 13px;
      button {
        width: 60px;
        height: 30px;
        border-radius: 20px;
        font-size: 12px;
        background-color: rgb(25, 45, 37);
        border: #fff;
        color: #fff;
      }
    }
  }
}
</style>
