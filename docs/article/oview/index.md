#  

<div style="display:flex;align-items:center;justify-content:center;flex-direction: column;margin-bottom:40px;flex:1">
<img src="/images/oview/logo.png">
<p style="font-size: 28px;font-weight: 500;">oView Vue.js移动端图表库</p>
<div style="display:flex;justify-content:center;">

<a href="https://github.com/MrGaoGang/oview">
<img src="https://img.shields.io/badge/github-%E4%BB%A3%E7%A0%81%E5%9C%B0%E5%9D%80-brightgreen.svg"/>
</a>

<a href="https://mrgaogang.github.io/oview/docs/#/" style="margin-left:30px;">
<img src="https://img.shields.io/badge/%E5%AE%98%E6%96%B9%E7%A4%BA%E4%BE%8B-%E6%95%88%E6%9E%9C%E5%9B%BE-%232d8cf0.svg"/>
</a>
</div>
<img src="/images/oview/qrcode.png" style="wdith:150px;height:150px">

</div>

> oView是基于 [蚂蚁金服F2](https://www.yuque.com/antv/f2/getting-started)图表库的二次封装，以便于Vue.js开发者在移动端和PC端更好进行图表的展示。


**NPM安装**

```
npm install oview --save

```
> 推荐使用npm安装，享受安装依赖包带来的便利，同时也建议使用个人开发Vue项目使用的 [Vue SPA 模板](https://github.com/MrGaoGang/lucky_vue_template);当然Vue官方提供的cli模板固然优秀，但是由于加重了学习成本，所以对有webpack开发经验的同学使用此模板，可尽快入手。



**oView特性**

- **1、oview支持哪些图？**
    **目前oview支持：柱状图，饼状图，面积图，散点图，气泡图，面积图，折线图 ，雷达图，自定义图**

- **2、图表配置简单**

    ```html
    <!-- 没错，配置一个饼状图就是这么简单--->
    <o-chart :data="data">
      <o-pie position="name*percent"></o-pie>
    </o-chart>
    ```
    如果您只需要，配置简单的图形，只需要传递数据，和坐标轴即可。

- **oview图表色彩鲜艳**

> 色彩主要使用F2官方建议色彩，如需自定义色彩可使用:color="yourColors"传入即可。（后续会详细讲解）

<div style="display:flex;justify-content:space-around;">
<img src="/images/oview/oview_main.png" style="width:300px;height:600px"/>

<img src="/images/oview/oview_pie.png" style="width:300px;height:600px"/>

</div>


## [饼状图](./chart/pie.md)
## [柱状图](./chart/histo.md)
## [折线图](./chart/line.md)
## [雷达图](./chart/radar.md)
## [散点图和气泡图](./chart/point.md)
## [面积图](./chart/area.md)
## [图片平移缩放](./chart/intercation.md)