<template>
  <body>
    <div>
      <div class="top">
        <div class="top_left">
          <img src="../img/图层 2.png" alt="">
          <div class="wei">
            <div><span class="iconfont">&#xe66e;</span><span>运行监控</span></div>
          </div>
          <div>
            <div><span class="iconfont">&#xe675;</span><span>生产管理</span></div>
          </div>
          <div>
            <div><span class="iconfont">&#xe676;</span><span>电站维护</span></div>
          </div>
          <div>
            <div><span class="iconfont">&#xe67d;</span><span>系统管理</span></div>
          </div>
        </div>
        <div class="top_right">
          <p>16:27</p>
          <p>|</p>
          <p>2016-07-26</p>
          <div></div>
          <p>Jason</p>
          <span class="iconfont">&#xe82f;</span>
          <span class="iconfont">&#xe86b;</span>
          <span class="iconfont">&#xe869;</span>
        </div>
      </div>
      <div class="below">
        <div class="below_left">
          <ul>
            <li class="wei"><span class="iconfont">&#xe630;</span><span>首页</span></li>
            <li><span class="iconfont">&#xe8c5;</span><span>电力监控</span></li>
            <li><span class="iconfont">&#xeb37;</span><span>光伏区监控</span></li>
            <li><span class="iconfont">&#xeb59;</span><span>设备分布图</span></li>
            <li><span class="iconfont">&#xe667;</span><span>设备实时数据</span></li>
            <li><span class="iconfont">&#xf02fe;</span><span>故障告警</span></li>
            <li><span class="iconfont">&#xf00a7;</span><span>远程控制</span></li>
          </ul>
        </div>
        <div class="below_right">
          <div class="below_top div_1">
            <div><span class="iconfont">&#xf0210;</span><span>发电与功率</span></div>
            <div class="main1" style="  background-color: #1a194f;">
              <div v-for="item in arr" style="padding:5% 0;   ">
                <div style="margin: auto; width:80%;display: flex;">
                  <div class="round" :style="{ 'background-color': item.color }"></div>
                  <div style="width: 80%; display: flex; flex-wrap:wrap ;justify-content:space-evenly">
                    <p style="margin-left:10px ;">{{ item.text }}</p>
                    <div style="display: flex;">
                      <p :style="{ 'color': item.color, 'textAlign': 'right', 'margin': '0px 5px' }">{{ item.shuzi }}</p>
                      <p style="text-align: right;">kw/h</p>
                    </div>
                    <div
                      :style="{ 'width': '100%', 'height': '10px', 'backgroundColor': '#fff7', 'border-radius': '5px', margin: '0px 0px 0px 20px' }">
                      <div
                        :style="{ 'width': item.width, 'height': '100%', 'backgroundColor': item.color, 'border-radius': '5px' }">
                      </div>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
          <div class="below_top div_2">
            <div><span class="iconfont">&#xe60b;</span><span>节能减排</span></div>
            <div class="main4"
              style="display: flex; justify-content:space-between;margin:0px 20px;background-color: #1a194f;height:80% ;">
              <div style="display: flex;flex-direction:column;justify-content:space-around">
                <p>二氧化碳</p>
                <p>汽车里程</p>
                <p>等效植树</p>
                <p>二氧化硫</p>
              </div>
              <div style="display: flex;flex-direction:column;justify-content:space-around">
                <div style="display: flex;justify-content:space-between;width:130px">
                  <p style="font-size:26px ;font-weight:600 ;">8.45</p>
                  <p style="line-height: 35px;">万吨</p>
                </div>
                <div style="display: flex;justify-content:space-between;width:130px">
                  <p style="font-size:26px ;font-weight:600 ;">7.37</p>
                  <p style="line-height: 35px;">km</p>
                </div>
                <div style="display: flex;justify-content:space-between;width:130px">
                  <p style="font-size:26px ;font-weight:600 ;">461.79</p>
                  <p style="line-height: 35px;">万吨</p>
                </div>
                <div style="display: flex;justify-content:space-between;width:130px">
                  <p style="font-size:26px ;font-weight:600 ;">2542.91</p>
                  <p style="line-height: 35px;">吨</p>
                </div>
              </div>
            </div>
          </div>
          <div class="below_top div_3">
            <div><span class="iconfont">&#xe61f;</span><span>电站基本信息</span></div>
            <div class="main5"
              style="display: flex; justify-content:space-between;margin:0px 20px;background-color: #1a194f;height:80% ;">
              <div style="display: flex;flex-direction:column;justify-content:space-around;align-items:flex-start">
                <div style="display: flex;">
                  <div class="dian"></div>
                  <p>电站名称</p>
                </div>
                <div style="display: flex;">
                  <div class="dian"></div>
                  <p>精度/维度</p>
                </div>
                <div style="display: flex;">
                  <div class="dian"></div>
                  <p>装机功率</p>
                </div>
                <div style="display: flex; ">
                  <div class="dian"></div>
                  <p>组件数量</p>
                </div>
                <div style="display: flex;">
                  <div class="dian"></div>
                  <p>电站类型</p>
                </div>
                <div style="display: flex;">
                  <div class="dian"></div>
                  <p>投运时间</p>
                </div>
                <div style="display: flex;">
                  <div class="dian"></div>
                  <p>生命周期</p>
                </div>
              </div>
              <div style="display: flex;flex-direction:column;justify-content:space-around">
                <p>三十岗电站</p>
                <p>东经117° 北纬23°</p>
                <p>123.23kw</p>
                <p>2000块</p>
                <p>分布式电站</p>
                <p>2018年05月10日</p>
                <p>25年</p>
              </div>
            </div>
          </div>
          <div class="below_below div_4">
            <div><span class="iconfont">&#xe6c1;</span><span>日功率-辐射强度</span></div>
            <div class="main2" style="height:80%; margin: auto;width:100%;background-color: #1a194f;">

            </div>
          </div>
          <div class="below_below div_5">
            <div><span class="iconfont">&#xe771;</span><span>日累计发电量</span></div>
            <div class="main3" style="height:80%; margin: auto;width:100%;background-color: #1a194f;"></div>
          </div>
        </div>
      </div>
    </div>
  </body>
</template> 


<style>
@font-face {
  font-family: 'iconfont';
  src: url('iconfont.ttf?t=1704157471372') format('truetype');
}

.iconfont {

  font-family: "iconfont" !important;
  font-size: 24px;
  font-style: normal;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

* {
  margin: 0px;
  padding: 0px;
}

html {
  height: 100%;
}

body {
  height: 100%;
}

body>div {
  margin: 0px;
  padding: 0px;
  width: 100%;
  height: 100%;
  margin: auto;
  display: flex;
  flex-direction: column;
}

.top {
  background-color: #27265c;
  color: rgb(255, 255, 255);
  display: flex;
  justify-content: space-between;
  height: 80px;
  width: 100%;
  overflow-y: hidden;
}

.top_left {
  display: flex;
  width: 50%;
}

.top_left>div {
  width: 20%;
  margin: auto;
  display: flex;
  justify-content: space-around;
}

.iconfont {
  position: relative;
  top: 3px;
}

.top_left>div>div>span {
  text-align: center;
  line-height: 65px;
}

.top_left>img {
  min-width: 200px;
  width: 200px;
}

.top_left>.wei {
  border-bottom: 3px solid #884336;
  background-color: #0b0e40;
}

.top_right {
  display: flex;
  color: #c7c7c7;
}

.top_right>p {
  text-align: center;
  line-height: 75px;
  margin: 0px 10px;
}

.top_right>span {
  text-align: center;
  line-height: 75px;
  margin: 0px 15px;
}

.top_right>div {
  background-color: #000000;
  height: 50px;
  width: 50px;
  border: 1px solid #fff;
  border-radius: 50%;
  margin: auto;
}

.below {
  background-color: #0b0e40;
  flex: 1;
  display: flex;
  color: #fff;

}

.below_left {
  background-color: #27265c;
  width: 200px;
  min-width: 200px;
}

.below_left>ul>li {
  height: 60px;
  line-height: 55px;
}

.below_left>ul>li>span {
  margin: 0px 5px;
}

.below_left>ul>li>.iconfont {
  position: relative;
  top: 3px;
  margin-left: 30px;
}

.below_left .wei {
  background-image: linear-gradient(90deg, #0b0e40, #27265c);
}

.below_right {
  display: flex;
  flex-wrap: wrap;
  align-content: space-around;
  width: 100%;
  height: 100%;
}

.below_right>div {
  background-color: #1a194f;
  margin: 10px 0px 10px 20px;
  height: 45%;
}

.below_top {
  width: 31.5%;
}

.below_below {
  width: 48%;
}

.below_top>div>span {
  line-height: 50px;
  margin: 0px 15px;
}

.below_top>div>.iconfont {
  position: relative;
  top: 3px;
}

.below_top>div {
  background-color: #27265c;
}

.below_below>div>span {
  line-height: 50px;
  margin: 0px 15px;
}

.below_below>div>.iconfont {
  position: relative;
  top: 3px;
}

.below_below>div {
  background-color: #27265c;
  height: 60px;
}

.main1 {
  width: 100%;
  margin: auto;
}

.round {
  width: 50px;
  height: 50px;
  border-radius: 50%;
}

.dian {
  width: 5px;
  height: 5px;
  border-radius: 50%;
  background-color: aqua;
  margin: auto;
  margin-right: 10px;
}
</style>


<script>
import * as echarts from 'echarts';
export default {
  name: 'Login',
  data() {
    return {
      form: {
        name: '',
        password: '',
      },
      arr: [
        { text: '累计发电', color: '#f7f71d', shuzi: '123589256.00', width: '80%' },
        { text: '今日发电', color: '#7bc1ef', shuzi: '4567.00', width: '50%' },
        { text: '当前功率', color: '#b94ecb', shuzi: '567.00', width: '20%' },
      ]
    }
  },
  mounted() {
    setTimeout(() => {
      var myChart1 = echarts.init(document.getElementsByClassName('main2')[0]);
      myChart1.setOption({
        color: ['#0E8DAD', '#8524AF'],
        tooltip: {
          trigger: 'axis',
          axisPointer: {
            type: 'cross',
            label: {
              backgroundColor: '#0E8DAD'
            }
          }
        },
        grid: {
          left: '3%',
          right: '4%',
          bottom: '3%',
          containLabel: true
        },
        xAxis: [
          {
            type: 'category',
            boundaryGap: false,
            data: [3, 6, 9, 12, 15, 18, 21, 24]
          }
        ],
        yAxis: [
          {
            type: 'value'
          }
        ],
        series: [
          {
            name: 'Line 1',
            type: 'line',
            stack: 'Total',
            smooth: true,
            lineStyle: {
              width: 0
            },
            showSymbol: false,
            areaStyle: {
              opacity: 0.8,
              color: new echarts.graphic.LinearGradient(0, 0, 0, 1, [
                {
                  offset: 0,
                  color: '#0E8DAD'
                },
                {
                  offset: 1,
                  color: '#8524AF'
                }
              ])
            },
            emphasis: {
              focus: 'series'
            },
            data: [140, 232, 101, 264, 90, 340, 250, 340]
          },
          {
            name: 'Line 2',
            type: 'line',
            stack: 'Total',
            smooth: true,
            lineStyle: {
              width: 0
            },
            showSymbol: false,
            areaStyle: {
              opacity: 0.8,
              color: new echarts.graphic.LinearGradient(0, 0, 0, 1, [
                {
                  offset: 0,
                  color: 'rgb(0, 221, 255)'
                },
                {
                  offset: 1,
                  color: 'rgb(77, 119, 255)'
                }
              ])
            },
            emphasis: {
              focus: 'series'
            },
            data: [120, 282, 111, 234, 220, 340, 310, 110]
          }
        ]

      });
      var myChart2 = echarts.init(document.getElementsByClassName('main3')[0]);
      myChart2.setOption({
        color: ['#0E8DAD', '#8524AF'],
        grid: {
          left: '3%',
          right: '4%',
          bottom: '3%',
          containLabel: true
        },
        xAxis: {
          type: 'category',
          data: ['3', '6', '9', '12', '15', '18', '21', '24']
        },
        yAxis: {
          type: 'value',
        },
        series: [
          {
            data: [120, 200, 150, 80, 70, 110, 130, 80],
            type: 'bar'
          }, {
            data: [120, 200, 150, 80, 70, 110, 130, 90],
            type: 'bar'
          },
        ]
      })
    }, 0); // 设置延迟时间为0，确保在下一次事件循环中执行
  }
}
</script>

