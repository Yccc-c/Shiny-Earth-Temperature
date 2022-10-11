# 地表温度可视化

本文主要研究地表温度数据的地图可视化操作，并通过对不同数据的简单分析，得出有关地表温度变化趋势及其分布特征的结论。

- 浏览Shiny程序[**点击这里**](http://shiny.csu.wiki/EarthTemp/EarthTemp-shiny)

本文全部内容使用<span style="color:lightblue">R语言</span>及Rstudio编写，数据集来自于[Kaggle](https://www.kaggle.com/datasets/berkeleyearth/climate-change-earth-surface-temperature-data)。

本文所使用的地图数据集来源如下：

1. 世界地图：源自`ggplot2::map_data("world")`
2. 澳大利亚、巴西、加拿大、印度、俄罗斯、美国一级行政区边界数据：[**GADM**](https://gadm.org/index.html)。其版权说明如下：

> The data are freely available for academic use and other non-commercial use. Redistribution or commercial use is not allowed without prior permission.

3. 中国地图数据：[**Horizon**](http://horizon2021.xyz/)

> 本文依赖的[Shiny程序](http://shiny.csu.wiki/EarthTemp/EarthTemp-shiny)使用[**flexdashboard**](https://pkgs.rstudio.com/flexdashboard/)包制作。因数据量大以及服务器运算量限制，每次访问该Shiny程序时需要加载约一分钟时间，请耐心等待。同时因流式页面的特性，每次缩放浏览器窗口都会令Shiny重新运行并绘制图像，故请您务必不要多次改变窗口大小，以免网站崩溃。如遇网站崩溃，还请及时联系站长：*cheny_ycc@qq.com*。

- 本仓库共有两个代码文件：
  - Dashboard.Rmd：Shiny主程序代码
  - EarthTemp.Rmd：实验报告
