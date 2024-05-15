<template>
  <div class="home">
    <dv-border-box-8>
      <dv-decoration-5 style="width: 100%; height: 130px" class="a"></dv-decoration-5>
      <PieChart></PieChart>
      <HarvestTwo></HarvestTwo>
    </dv-border-box-8>
  </div>
</template>

<script>
// @ is an alias to /src
import PieChart from "@/components/PieChart.vue"
import HarvestTwo from "@/components/HarvestTwo.vue"
export default {
  components: {
    PieChart,
    HarvestTwo
  }
}
</script>
<style lang="scss" scoped>
.home {
  width: 100vw;
  height: 100vh;
  background-image: url(../assets/百香果数字运营中心/bg\(1\).png);
  background-size: cover;
  background-repeat: no-repeat;
  background-position: 0 -19px;

  .a {
    background-image: url(../assets/百香果数字运营中心/标题.png);
    background-size: cover;
    background-repeat: no-repeat;
  }
}
</style>
