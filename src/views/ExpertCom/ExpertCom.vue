<template>
  <div class="Expert-box">
    <!-- 第一个图片 -->
    <div class="img">
      <div class="image">
        <img src="../../assets/imgs/组 3038@3x.png" alt="" />
        <span>51</span>
      </div>
      <p>23123123</p>
    </div>
    <div class="img">
      <div class="image">
        <img src="../../assets/imgs/组 3038@3x(1).png" alt="" />
        <span>66</span>
      </div>
      <p>23123123</p>
    </div>
    <div class="img">
      <div class="image">
        <img src="../../assets/imgs/组 3038@3x(2).png" alt="" />
        <span>96</span>
      </div>
      <p>23123123</p>
    </div>
  </div>
</template>
<script>
export default {
  components: {},
  data() {
    return {}
  },
  methods: {}
}
</script>
<style lang="scss">
.Expert-box {
  width: 100%;
  height: 100%;
  background-color: #317f786f;
  box-shadow: inset 1px 1px 20px #11211c;
  border-radius: 10px;
  // float: right;
  display: flex;
  align-items: center;
  justify-content: space-around;
  .img {
    height: 80px;
    display: flex;
    text-align: center;
    flex-direction: column;
    justify-content: space-around;
    color: #fff;
    font-size: 14px;
    .image {
      position: relative;
      img {
        width: 100px;
        height: 50px;
      }
      span {
        position: absolute;
        top: 50%;
        margin-top: -6px;
        left: 50%;
        margin-left: 8px;
      }
    }
  }
}
</style>
