<template>
  <dv-full-screen-container class="home">
    <div class="decoration"><img src="../assets/imgs/标题.png" alt="" /></div>
    <div class="main">
      <div class="box"><OutLine /></div>
      <div class="box">2</div>
      <div class="box">3</div>
      <div class="box">
        <Scientific />
      </div>
      <div class="box">5</div>
      <div class="box">6</div>
      <div class="box">7</div>
      <div class="box"></div>
      <div class="box"></div>
      <div class="box">10</div>
    </div>
  </dv-full-screen-container>
</template>
<script>
import OutLine from "@/components/OutLine.vue"
import Scientific from "@/components/ScientificMap.vue"
export default {
  components: { OutLine, Scientific },
  data() {
    return {}
  }
}
</script>
<style lang="scss" scoped>
.home {
  width: 100vw;
  height: 100vh;
  background-image: url(../assets/imgs/bg\(1\).png);
  background-size: 100% 100%;
  background-repeat: no-repeat;
  background-position: 0 -19px;
  position: relative;

  .decoration {
    width: 100%;
    height: 100px;

    img {
      width: 100%;
    }
  }
}
.main {
  padding: 0 10px;
  height: 100vh;
  display: grid;
  grid-template:
    "a a a d d d d d e e e" 1fr
    "a a a d d d d d e e e" 1fr
    "a a a d d d d d f f f" 1fr
    "a a a d d d d d f f f" 1fr
    "b b b d d d d d f f f" 1fr
    "b b b d d d d d g g g" 1fr
    "b b b d d d d d g g g" 1fr
    "b b b d d d d d g g g" 1fr
    "b b b i i i j j h h h" 1fr
    "c c c i i i j j h h h" 1fr
    "c c c i i i j j h h h" 1fr
    /1fr 1fr 1fr 1fr 1fr 1fr 1fr 1fr 1fr 1fr 1fr;
  grid-gap: 10px;
}
.main > .box {
  background-color: #23555388;
  color: white;
  border-radius: 10px;
  box-shadow: inset 1px 1px 20px 4px #4d9276;
  box-sizing: border-box;
}
.main > .box:nth-of-type(1) {
  grid-area: a;
  border-radius: 5px;
}
.main > .box:nth-of-type(2) {
  grid-area: b;
}
.main > .box:nth-of-type(3) {
  grid-area: c;
}
.main > .box:nth-of-type(4) {
  grid-area: d;
  background-color: transparent;
  border: none;
  box-shadow: none;
}

.main > .box:nth-of-type(5) {
  grid-area: e;
}
.main > .box:nth-of-type(6) {
  grid-area: f;
}
.main > .box:nth-of-type(7) {
  grid-area: g;
}
.main > .box:nth-of-type(8) {
  grid-area: h;
}
.main > .box:nth-of-type(9) {
  grid-area: i;
}
.main > .box:nth-of-type(10) {
  grid-area: j;
}
</style>
