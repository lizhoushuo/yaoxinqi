<template>
  <main class="scientific">
    <!-- 第一块 -->
    <div class="item" @mouseenter="flag = true" @mouseleave="flag = false">
      <img src="../assets/imgs/组 230@3x(1).png" alt="" v-if="flag" />
      <img src="../assets/imgs/组 230@3x.png" alt="" v-else />
      <div v-if="flag" style="color: #caae34">
        <div class="item-title">科研地块</div>
        <div class="item-desc">富强1号</div>
      </div>
      <div v-else>
        <div class="item-title">科研地块</div>
        <div class="item-desc">富强1号</div>
      </div>
      <div class="modal" v-show="flag">
        <div class="top">
          <img src="../assets/imgs/容器 47@3x.png" alt="" />
          <font style="color: #caae34">科研地块3 【京都3号】</font>
        </div>
        <div class="aside">
          <img src="../assets/imgs/蒙版组 3@3x.png" alt="" />
          <img src="../assets/imgs/蒙版组 6@3x.png" alt="" />
        </div>
        <div class="footer">扫码查看种植过程</div>
      </div>
    </div>
    <!-- 第二块 -->
    <div class="item1" @mouseenter="flag1 = true" @mouseleave="flag1 = false">
      <img src="../assets/imgs/组 230@3x(1).png" alt="" v-if="flag1" />
      <img src="../assets/imgs/组 230@3x.png" alt="" v-else />
      <div v-if="flag1" style="color: #caae34">
        <div class="item-title">科研地块</div>
        <div class="item-desc">民主2号</div>
      </div>
      <div v-else>
        <div class="item-title">科研地块</div>
        <div class="item-desc">民主2号</div>
      </div>
      <div class="modal" v-show="flag1">
        <div class="top">
          <img src="../assets/imgs/容器 47@3x.png" alt="" />
          <font style="color: #caae34">科研地块3 【京都3号】</font>
        </div>
        <div class="aside">
          <img src="../assets/imgs/蒙版组 3@3x.png" alt="" />
          <img src="../assets/imgs/蒙版组 6@3x.png" alt="" />
        </div>
        <div class="footer">扫码查看种植过程</div>
      </div>
    </div>

    <!-- 第三块 -->
    <div class="item2" @mouseenter="flag2 = true" @mouseleave="flag2 = false">
      <img src="../assets/imgs/组 230@3x(1).png" alt="" v-if="flag2" />
      <img src="../assets/imgs/组 230@3x.png" alt="" v-else />
      <div v-if="flag2" style="color: #caae34">
        <div class="item-title">科研地块</div>
        <div class="item-desc">文明3号</div>
      </div>
      <div v-else>
        <div class="item-title">科研地块</div>
        <div class="item-desc">文明3号</div>
      </div>
      <div class="modal" v-show="flag2">
        <div class="top">
          <img src="../assets/imgs/容器 47@3x.png" alt="" />
          <font style="color: #caae34">科研地块3 【京都3号】</font>
        </div>
        <div class="aside">
          <img src="../assets/imgs/蒙版组 3@3x.png" alt="" />
          <img src="../assets/imgs/蒙版组 6@3x.png" alt="" />
        </div>
        <div class="footer">扫码查看种植过程</div>
      </div>
    </div>
    <!-- 第四块 -->
    <div class="item3" @mouseenter="flag3 = true" @mouseleave="flag3 = false">
      <img src="../assets/imgs/组 230@3x(1).png" alt="" v-if="flag3" />
      <img src="../assets/imgs/组 230@3x.png" alt="" v-else />
      <div v-if="flag3" style="color: #caae34">
        <div class="item-title">科研地块</div>
        <div class="item-desc">和谐号</div>
      </div>
      <div v-else>
        <div class="item-title">科研地块</div>
        <div class="item-desc">和谐号</div>
      </div>
      <div class="modal" v-show="flag3">
        <div class="top">
          <img src="../assets/imgs/容器 47@3x.png" alt="" />
          <font style="color: #caae34">科研地块3 【京都3号】</font>
        </div>
        <div class="aside">
          <img src="../assets/imgs/蒙版组 3@3x.png" alt="" />
          <img src="../assets/imgs/蒙版组 6@3x.png" alt="" />
        </div>
        <div class="footer">扫码查看种植过程</div>
      </div>
    </div>
  </main>
</template>
<script>
export default {
  data() {
    return {
      flag: false,
      flag1: false,
      flag2: false,
      flag3: false
    }
  },
  methods: {}
}
</script>
<style lang="scss" scoped>
.scientific {
  width: 100%;
  height: 100%;
  position: relative;
  img {
    width: 44px;
    height: 33px;
  }
  .item {
    position: absolute;
    top: 22px;
    left: 130px;
    // position: relative;
    .modal {
      position: absolute;
      top: -50px;
      left: 65px;
    }
  }
  .item1 {
    position: absolute;
    top: 150px;
    left: 200px;
    // position: relative;
    .modal {
      position: absolute;
      top: -25px;
      left: -175px;
    }
  }
  .item2 {
    position: absolute;
    right: 125px;
    bottom: 105px;
    // position: relative;
    .modal {
      position: absolute;
      right: -75px;
      bottom: 75px;
    }
  }
  .item3 {
    position: absolute;
    left: 260px;
    bottom: 95px;
    .modal {
      position: absolute;
      right: 70px;
      bottom: -60px;
    }
  }
}
.modal {
  box-sizing: border-box;
  font-size: 12px;
  // padding:0 10px;
  background-color: #00000096;
  border-radius: 10px;
  .top {
    padding: 5px;
    color: #c0ab38;
    display: flex;
    align-items: center;
    border-bottom: 1px solid #c0ab38;
    img {
      margin-right: 5px;
      width: 10px;
      height: 10px;
    }
  }
  .aside {
    display: flex;
    justify-content: center;
    padding: 5px;
    img {
      width: 70px;
      height: 70px;
      margin: 5px;
    }
  }
  .footer {
    text-align: center;
    padding: 5px 0;
  }
}
</style>
