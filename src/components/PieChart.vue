<template>
  <div class="box">
    <div class="title">
      <img src="../assets/imgs/容器 47@2x.png" alt="" />
      <div class="tit">土壤肥力分析</div>
    </div>
    <div class="nn">
      <div id="myChart2" style="width: 100%; height: 100%"></div>
    </div>
  </div>
</template>

<script>
import * as echarts from "echarts"
export default {
  components: {},
  data() {
    return {}
  },
  computed: {},
  watch: {},

  mounted() {
    this.echart()
  },
  methods: {
    echart() {
      let myChart = echarts.init(document.getElementById("myChart2"))
      var colorList = ["#73DDFF", "#73ACFF", "#FDD56A", "#FDB36A", "#FD866A", "#9E87FF", "#58D5FF"]
      var arr = [
        { value: 123, name: "丙烯腈" },
        { value: 102, name: "环氧乙烷" },
        { value: 122, name: "非甲烷总烃" },
        { value: 137, name: "氯乙烯" },
        { value: 109, name: "氯乙烷" },
        { value: 111, name: "甲苯" }
      ]
      myChart.setOption({
        color: colorList,

        tooltip: {
          trigger: "item"
        },
        series: [
          {
            type: "pie",
            center: ["50%", "50%"],
            radius: ["50%", "60%"],
            height: 130,
            clockwise: true,
            avoidLabelOverlap: true,
            hoverOffset: 15,
            itemStyle: {
              normal: {
                color: function (params) {
                  return colorList[params.dataIndex]
                }
              }
            },
            label: {
              show: true,
              position: "outside",
              formatter: "{a|{b}：{d}%}\n{hr|}",
              rich: {
                a: {
                  padding: [0, -100, 0, -100]
                }
              }
            },
            labelLine: {
              normal: {
                length: 1,
                length2: 120,
                lineStyle: {
                  width: 1
                }
              }
            },
            data: arr
          }
        ]
      })
    }
  }
}
</script>

<style scoped>
.box {
  width: 100%;
  height: 100%;
  color: white;
  border-radius: 10px;
  box-sizing: border-box;
}

.title {
  box-sizing: border-box;
  width: 100%;
  padding: 10px;
  border-bottom: 1px solid #4d9276;
  display: flex;
  align-items: center;
  margin-bottom: 10px;
}

.tit {
  margin-left: 10px;
  /* font-weight: 700; */
  transform: skew(-10deg, 0deg);
  font-size: 14px;
  letter-spacing: 5px;
}
.nn {
  width: 100%;
}
</style>
