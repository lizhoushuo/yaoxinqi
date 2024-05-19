<template>
  <div class="box">
    <div class="title">
      <div class="l">
        <img src="../assets/imgs/容器 47@3x.png" alt="" />
        <div class="tit">收成详情</div>
      </div>
      <div class="btn">
        <div @click="flag = 0" :class="flag == 0 ? 'active' : 'bt1'">预计</div>
        <div @click="flag = 1" :class="flag == 1 ? 'active2' : 'bt2'">实际</div>
      </div>
    </div>
    <div class="cont">
      <div class="jgq">
        <div class="it">
          <div class="dec">果实</div>
          <div class="end">百香果</div>
        </div>
        <div class="it">
          <div class="dec">预计收成</div>
          <div class="end">491斤</div>
        </div>
        <div class="it">
          <div class="dec">预计收费</div>
          <div class="end">569198元</div>
        </div>
      </div>
      <div class="hr"></div>
      <div class="jgh">
        <div class="it">
          <div class="dec">加工后</div>
          <div class="end">百香果酱</div>
        </div>
        <div class="it">
          <div class="dec">预计收成</div>
          <div class="end">200斤</div>
        </div>
        <div class="it">
          <div class="dec">价格</div>
          <div class="end">29/斤</div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  components: {},
  data() {
    return {
      flag: 0
    }
  },
  computed: {},
  watch: {},
  methods: {}
}
</script>

<style scoped>
.box {
  width: 100%;
  height: 100%;
  background-color: #23555388;
  color: white;
  border-radius: 10px;
  box-shadow: inset 1px 1px 20px 4px #4d9276;
  box-sizing: border-box;
}

.title {
  box-sizing: border-box;
  width: 100%;
  height: 30%;
  /* padding: 20px 30px; */
  border-bottom: 1px solid #4d9276;
  display: flex;
  align-items: center;
  margin-bottom: 10px;
  justify-content: space-between;
}

.l {
  width: 48%;

  /* width: 16px; */
  height: 16px;
  display: flex;
  align-items: center;
}
.l img {
  height: 16px;
  /* width: 100%; */
  width: 16px;
}
.tit {
  width: 48%;
  font-weight: 700;
  transform: skew(-10deg, 0deg);
  font-size: 16px;
  letter-spacing: 5px;
}

.btn {
  display: flex;
  align-items: center;
}

.bt1,
.bt2 {
  box-sizing: border-box;
  border: 1px solid #36685bb7;
  padding: 6px 10px;
  box-shadow: inset 1px 1px 20px 4px #4d927698;
  font-size: 14px;
  cursor: pointer;
}

.bt1 {
  border-radius: 20px 0 0 20px;
}

.bt2 {
  border-radius: 0 20px 20px 0;
}

.active {
  padding: 6px 10px;
  border-radius: 20px 0 0 20px;
  border-color: rgba(238, 192, 117, 0.719);
  box-shadow: rgb(252 220 107 / 60%) 3px 0px 20px 4px inset;
  font-size: 14px;
}

.active2 {
  padding: 6px 10px;
  border-radius: 0 20px 20px 0;
  border-color: rgba(238, 192, 117, 0.719);
  box-shadow: rgb(252 220 107 / 60%) 3px 0px 20px 4px inset;
  font-size: 14px;
}

.cont {
  box-sizing: border-box;
  width: 100%;
  padding: 0 30px;
}

.jgq,
.jgh {
  display: flex;
  justify-content: space-between;
}

.end {
  margin-top: 6px;
  color: #ccda92;
  font-weight: 700;
}

.dec {
  font-size: 14px;
}

.hr {
  width: 100%;
  height: 1px;
  background: linear-gradient(to right, #49776700, #2e9b75, #508f7900);
  margin: 20px;
}

.it {
  width: 30%;
  height: 50%;
}
</style>
