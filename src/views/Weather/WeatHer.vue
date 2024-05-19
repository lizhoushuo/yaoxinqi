<template>
  <div class="weather">
    <div class="weather-top"><img src="../../assets/imgs/容器 47@2x.png" alt="" /><span>天气预报</span></div>
    <div class="bb">
      <div class="weather-content">
        <div class="weather-content-time">
          <div><span>今天</span> <span>03/11</span></div>
          <div><img src="../../assets/imgs/83.png" alt="" /><span style="color: yellowgreen">晴</span></div>
          <div class="ww">
            <span>18°c</span>
            <div class="wendu"></div>
            <span>24°c</span>
          </div>
        </div>
      </div>
      <div class="weather-content">
        <div class="weather-content-time">
          <div><span>明天</span> <span>03/12</span></div>
          <div><img src="../../assets/imgs/83.png" alt="" /><span style="color: yellowgreen">晴</span></div>
          <div class="ww">
            <span>12°c</span>
            <div class="wendu2"></div>
            <span>30°c</span>
          </div>
        </div>
      </div>
      <div class="weather-content">
        <div class="weather-content-time">
          <div><span>周三</span> <span>03/13</span></div>
          <div><img src="../../assets/imgs/83.png" alt="" /><span style="color: yellowgreen">晴</span></div>
          <div class="ww">
            <span>16°c</span>
            <div class="wendu3">
              <div class="a"></div>
            </div>
            <span>32°c</span>
          </div>
        </div>
      </div>
      <div class="weather-content">
        <div class="weather-content-time">
          <div><span>周四</span> <span>03/14</span></div>
          <div><img src="../../assets/imgs/83.png" alt="" /><span style="color: yellowgreen">晴</span></div>
          <div class="ww">
            <span>12°c</span>
            <div class="wendu4"><div class="a"></div></div>
            <span>32°c</span>
          </div>
        </div>
      </div>
      <div class="weather-content">
        <div class="weather-content-time">
          <div><span>周五</span> <span>03/15</span></div>
          <div><img src="../../assets/imgs/83.png" alt="" /><span style="color: yellowgreen">晴</span></div>
          <div class="ww">
            <span>15°c</span>
            <div class="wendu5"><div class="a"></div></div>
            <span>26°c</span>
          </div>
        </div>
      </div>
      <div class="weather-content">
        <div class="weather-content-time">
          <div><span>周六</span> <span>03/16</span></div>
          <div><img src="../../assets/imgs/83.png" alt="" /><span style="color: yellowgreen">晴</span></div>
          <div class="ww">
            <span>13°c</span>
            <div class="wendu6"><div class="a"></div></div>
            <span>18°c</span>
          </div>
        </div>
      </div>
      <div class="weather-content">
        <div class="weather-content-time">
          <div><span>周日</span> <span>03/17</span></div>
          <div><img src="../../assets/imgs/83.png" alt="" /><span style="color: yellowgreen">晴</span></div>
          <div class="ww">
            <span>18°c</span>
            <div class="wendu7"><div class="a"></div></div>
            <span>20°c</span>
          </div>
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
.weather {
  width: 100%;
  height: 2.6316rem;
  .weather-top {
    width: 100%;
    height: 100%;
    display: flex;
    align-items: center;
    border-bottom: 1px solid #fff;
    font-size: 0.8125rem;
    padding: 0.625rem;
    box-sizing: border-box;
    color: #fff;
    img {
      margin-right: 0.625rem;
    }
  }
  .bb {
    height: calc(100% - 50%);
    display: flex;
    flex-direction: column;
    justify-content: space-around;
  }
  .weather-content {
    color: #fff;
    font-size: 0.75rem;
    padding: 0.625rem;
    box-sizing: border-box;
    .weather-content-time {
      display: flex;
      align-content: center;
      justify-content: space-between;
      span {
        display: inline-block;
        margin-right: 0.625rem;
      }
      img {
        vertical-align: middle;
        margin-right: 0.625rem;
      }
      .ww {
        display: flex;
        align-items: center;
      }
      .wendu {
        width: 70px;
        height: 7px;
        border-radius: 20px;
        border: 1px solid #ddcc6a;
        background: radial-gradient(circle at center, rgb(210, 199, 126) 20%, rgb(210, 199, 126) 30%, transparent 20%);
        margin-right: 10px;
      }
      .wendu2 {
        width: 70px;
        height: 7px;
        border-radius: 20px;
        border: 1px solid #ddcc6a;
        background: radial-gradient(circle at center, rgb(210, 199, 126) 50%, rgb(210, 199, 126) 60%, transparent 50%);
        margin-right: 10px;
      }

      .wendu3 {
        width: 70px;
        height: 7px;
        border-radius: 20px;
        border: 1px solid #ddcc6a;
        margin-right: 10px;
        position: relative;
        .a {
          width: 40px;
          height: 7px;
          background-color: #ddcc6a;
          position: absolute;
          right: 7px;
        }
      }
      .wendu4 {
        width: 70px;
        height: 7px;
        border-radius: 20px;
        border: 1px solid #ddcc6a;
        margin-right: 10px;
        position: relative;
        .a {
          width: 36px;
          height: 7px;
          background-color: #ddcc6a;
          position: absolute;
          right: 13px;
        }
      }
      .wendu5 {
        width: 70px;
        height: 7px;
        border-radius: 20px;
        border: 1px solid #ddcc6a;
        margin-right: 10px;
        position: relative;
        .a {
          width: 35px;
          height: 7px;
          background-color: #ddcc6a;
          position: absolute;
          right: 15px;
        }
      }
      .wendu6 {
        width: 70px;
        height: 7px;
        border-radius: 20px;
        border: 1px solid #ddcc6a;
        margin-right: 10px;
        position: relative;
        .a {
          width: 25px;
          height: 7px;
          background-color: #ddcc6a;
          position: absolute;
          right: 30px;
        }
      }
      .wendu7 {
        position: relative;
        width: 70px;
        height: 7px;
        border-radius: 20px;
        border: 1px solid #ddcc6a;
        margin-right: 10px;
        position: relative;
        .a {
          width: 20px;
          height: 7px;
          background-color: #ddcc6a;
          position: absolute;
          right: 35px;
        }
      }
    }
  }
}
</style>
