# Superset 资料合集
本列表起始于2022年2月23号。 

## Superset 是什么？(介绍给完全没接触过的朋友)
[Superset](https://github.com/apache/superset) 简单说就是一个数据可视化的工具。  
它本身并不存储数据，它需要有一个后端数据库提供数据，可以是 PostgreSQL/MySQL/ClickHouse 等等（支持好几十种）  

## Superset 长啥样？
https://github.com/apache/superset 官方仓库里有截图，这里就不再重复贴图了。   

## 这个仓库是什么？
这里是一个列表，存放 Superset 的各种教程，文章，视频等信息。  
（中文的资料优先，排在前面）  

## 这东西对你有啥用？
帮助你学习 Superset。  
## 为什么有这个表？
初次接触：我从2022年初开始接触 Superset（这个时间点的 Superset 最新版本是 1.4.1）。   
最终目的：用 Superset + ClickHouse 搭建一个仅供公司内部使用的数据面板。     
介绍：Superset 最终会由我司员工（做技术的+不做技术的都有）用来分析数据。    

**学习 Superset 过程中遇到的问题**：
1. Superset 官方英文文档有不少改进空间（比如完全没有讲怎么部署到正式环境）   
2. 中文资料搜一搜的确有，但一般都是旧版本的（比如0.37），而且比较零散（单篇文章）

**问题总结：**：
1. 新手想入门 Superset，找资料比较费劲。

**有哪些解决办法**：
1. 方法1：既然官方英文文档不太行，那么我们可以自己去补（这个我已经在做了）(总结：改进英文文档)
2. 方法2：把英文文档翻译成中文文档（帮助有限，官方文档本来就一般般，翻译成中文也不会解决啥问题，有这功夫不如去改官方的英文文档）
3. 方法3：做一个简单的资料列表，把一些质量较高的资料整理一下，方便翻阅。

**结论**：  
在3个解决办法里，我选`方法3`，所以做这个列表。     
我也会放一些自己原创的文章到这里。   

## 如何参与？（添加你认为高价值的资料到列表中）
请创建 Issue 或者直接发送  Pull Request。  

<!--
# 技巧
* 如果一个字段是 DateTime, 
-->

# 列表
（才刚开始弄，现在内容还比较少，欢迎补充）   

* [(英文) 阅读 Contributing 文档](https://github.com/apache/superset/blob/master/CONTRIBUTING.md)：点评：除了官网文档 (指 https://superset.apache.org/docs/intro )应该全部读完之外，最应该读的就是 Contributing 了，因为里面详细介绍了如果要开发的话，如何在本地搭建开发环境。对 Superset 的代码基本情况做了介绍。  

* [(中文) Superset 基本概念](doc/1.Basic-Concept.md): 原创内容，我直接写到 doc 目录里了。 

* [(中文) 书籍《Python+Superset：商业智能数据分析与实战》](https://item.jd.com/10044365591593.html)：我在写这个列表时搜了一下京东，只看到 Superset 有这一本中文图书，还没看过这本书，等看过了来写评价。

## Superset 创始人(唯一一个创始人) Maxime Beauchemin 的演讲
这里把创始人 Maxime Beauchemin 的视频单独用一个区域列出来。   
因为比起其他演讲者，创始人本人出场的视频更值得关注。   

## 视频1：[2019年6月17日 - 视频长度39分钟44秒 - 视频标题：The history and anatomy of Apache Superset](https://www.youtube.com/watch?v=24XDOkGJrEY)  
这篇演讲主要讲：  
* 开篇3分钟做个人介绍。
* 3-5分钟：介绍 Superset 的用途，介绍给完全没接触过 Superset 的人。   
* 5-7分钟：介绍 Superset 里某些功能
* 7-10分钟：介绍 Superset 的特点
* 10-15分钟：介绍 Superset 的历史
  * 2015 年夏天在 Airbnb 工作，有一个 3 天的 Hackerthon，当时忙 Airflow 忙了9个多月了，所以想在 Hackerthon 做点不同的事情。 
  数据基础设施团队当时在弄 Druid 的 Proof of Concept (POC)。 
  Druid 是一个数据库，特点是 in-memory, column-stored，分布式，可以快速扫描很多行数据，速度很快。   
  * 当时离开 Facebook 一阵子了，讲了一下 Facebook 内部的一个同类数据库叫 Scuba。
  * Scuba 有 backend 和 frontend，协同工作。
  * 而 Druid 这边虽然是个不错的数据库，但是完全没有任何 GUI。 
  * 当时 Druid 还不能 Speak SQL, 现在支持了。  
  * 3天 Hackerthon 之后有个小成品。
  * 项目差点挂了，因为 Druid 当时还是 POC 仅在 Airbnb 内部使用，不确定是否应该坚持使用 Druid 作为后端。
  * 因为当时内部主要用 Presto，所以周末想把项目也兼容一下 Presto，在实现时，觉得不如兼容所有 SQL Speaking Database。  
  * 之前考虑过的名字是 Panoramix 和 Caravel，因为种种原因最后没用这些名字。  
  * 最后选了 Superset 这个名字。  
* 15-17分钟：
  * 大概一年半后，Airbnb 决定大力发展 Druid，专门设立一个团队来做。 
  4个工程师+1个PM，开始推进 Superset 和 Druid。
  * 讲了一下怎么加入 Apache Foundation 的。 
* 17-18分钟：
  * 放了一张 Github 截图以及一些关键指标。
  * 在 Airbnb 内部替代了 Tableau。
  * 其他在用 Superset 的知名公司。
* 19-22分钟
  * 讲 Stack 包括前端 React 后端 Python Flask。  
* 22-26分钟
  * **Superset 的架构图** (很有帮助)
* 26-32分钟
  * Challenges。
  * Fast Pace Repo
  * Huge Dependency Tree
  * Release Management
* 33-36分钟
  * Roadmap
  * What's Next?

**短总结（不想看上面长文看这个就够了）**：
1. Superset 诞生于2015年夏季，当时作者 Maxime Beauchemin 在 Airbnb 工作。  
2. 当时办了一个三天的 Hackerthon，当时作者在弄 Airflow 已经9个月了，想干点别的。那时候 Airbnb 内部在搞一个叫做 Druid 的数据库，但是这个数据库没有任何的前端，作者之前在 Facebook 工作的时候，Facebook 内部有个工具叫 Scuba，用途和 Druid 类似，但是 Scuba 的体验比较好。于是作者想给 Druid 也做一个类似的前端。  
3. 视频22分钟处有一个架构图非常有帮助，如果是完全没接触过的新手，看这个图的帮助不大，但是如果接触了一阵子 Superset 并且自己部署过了，也把官方文档都刷了一遍，再回头看这个就明白了。

## 视频2：[2020年10月17日 - 视频长度40分钟2秒 - 视频标题：Apache Superset - A data visualization platform](https://www.youtube.com/watch?v=VEuBZqdSoHk)
A presentation from ApacheCon @Home 2020   

* 0-5分钟
  * 2014年：在 Airbnb 创建了 Apache Airflow。 
  * 2015年：也是在 Airbnb 创建了 Apache Superset。   
  * 2019年创建了一家公司叫 Preset。是一家基于 Superset 的公司。   
    * 提供的服务包括训练人员以及部署 Superset。
* 5-14分钟
  * 介绍 Superset，聊一下业界情况。 
* 16分钟：`[SIP-53] Public Roadmap` 公开的发展路线。
* 18分钟：社区。
* 20分钟：Demo 终于开始了。开一个 Dashboard 但是半天加载不了。
* 27分钟：终于开始演示了。由于屏幕的分辨率不高。

**短总结**
1. 虽然视频分辨率最高有1080p，实际上屏幕演示的部分还是非常模糊。
2. 总体来说这个视频没啥帮助。就随便聊聊那种。


