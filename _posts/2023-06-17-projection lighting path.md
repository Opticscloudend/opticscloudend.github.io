---
layout:     post
title:      [DMD芯片照明光路]
subtitle:   [照明光路]
date:       [2023-06-17]
author:    jackfy
header-img: img/blog_Lucy.jpg
catalog: true
tags:
    - DMD
    - F数
    - F数匹配
    
---
#### (1) 投影光路

   Boss直聘上发现很多公司做投影比较多，微型投影产品比较多，虽然我对DLP光路没设计过，但是曾经搞LCD投影照明光路，其实原理都差不多，都要考虑F/#匹配。
查了DMD芯片，其设计比LCD的要复杂一点；DMD的偏振角决定了成像镜头的F/#,也觉得了照明光路的F/#; TI 的DMD的一般off and on 转角 -+（10-17）degree。
例如：转角17度，那么F/#=1.6,一般取大一点为1.7；另外要求光瞳匹配，成像投影镜头一般要求物方远心，那么照明光路出射也要远心，也就是两个入桶和出瞳都在无穷远相互匹配。
这样照明光路的主光线入射到每个cell都平行的。这些设计还是比较难度，前面的LED准直，复眼聚光中继镜 还是比较简单。如图时RGB微投照明系统：
![image](https://github.com/Opticscloudend/opticscloudend.github.io/assets/131378528/8b79ef67-29c7-406f-99ff-be13ee5cb433)
![image](https://github.com/Opticscloudend/opticscloudend.github.io/assets/131378528/b9ea801b-4129-49d6-8cd2-97f3379ac84b)
![image](https://github.com/Opticscloudend/opticscloudend.github.io/assets/131378528/b95d6586-acff-4a94-ba33-5997278c1f9b)
![image](https://github.com/Opticscloudend/opticscloudend.github.io/assets/131378528/3ba43418-2141-4846-81bc-b6db0acdf25d)




这个优化的结构导入tracepro做光效和均匀度数据分析。另外还要成像设计。公差分析==


     

