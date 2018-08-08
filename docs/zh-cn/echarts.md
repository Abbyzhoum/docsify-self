### Echarts

##### 图形图表等可以使用Echarts，功能强大,评价✨✨✨

> 介绍

  ECharts，一个使用 JavaScript 实现的开源可视化库，可以流畅的运行在 PC 和移动设备上，兼容当前绝大部分浏览器（IE8/9/10/11，Chrome，Firefox，Safari等），底层依赖轻量级的矢量图形库 ZRender，提供直观，交互丰富，可高度个性化定制的数据可视化图表。

> 教程 

①   获取 ECharts

      通过命令行： npm install echarts --save   npm安装
                 yarn add echarts             yarn安装

      通过cdn引入：你可以在 cdnjs，npmcdn 或者国内的 bootcdn 上找到 ECharts 的最新版本。

②    引入ECharts

      <!DOCTYPE html>
        <html>
        <head>
            <meta charset="utf-8">
            <!-- 引入 ECharts 文件 -->
            <script src="echarts.min.js"></script>
        </head>
        </html>

③    绘制一个简单的图表

      在绘图前我们需要为 ECharts 准备一个具备高宽的 DOM 容器

      <body>
    <!-- 为 ECharts 准备一个具备大小（宽高）的 DOM -->
    <div id="main" style="width: 600px;height:400px;"></div>
    </body>

    然后就可以通过 echarts.init 方法初始化一个 echarts 实例并通过 setOption 方法生成一个简单的柱状图，下面是完整代码。

      <!DOCTYPE html>
      <html>
      <head>
          <meta charset="utf-8">
          <title>ECharts</title>
          <!-- 引入 echarts.js -->
          <script src="echarts.min.js"></script>
      </head>
      <body>
          <!-- 为ECharts准备一个具备大小（宽高）的Dom -->
          <div id="main" style="width: 600px;height:400px;"></div>
          <script type="text/javascript">
              // 基于准备好的dom，初始化echarts实例
              var myChart = echarts.init(document.getElementById('main'));

              // 指定图表的配置项和数据
              var option = {
                  title: {
                      text: 'ECharts 入门示例'
                  },
                  tooltip: {},
                  legend: {
                      data:['销量']
                  },
                  xAxis: {
                      data: ["衬衫","羊毛衫","雪纺衫","裤子","高跟鞋","袜子"]
                  },
                  yAxis: {},
                  series: [{
                      name: '销量',
                      type: 'bar',
                      data: [5, 20, 36, 10, 10, 20]
                  }]
              };

              // 使用刚指定的配置项和数据显示图表。
              myChart.setOption(option);
          </script>
      </body>
      </html>

⑤     详情参考官网😯
          http://echarts.baidu.com/
