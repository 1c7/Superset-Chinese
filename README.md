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
1. 既然官方英文文档不太行，那么我们可以自己去补（这个我已经在做了）(总结：改进英文文档)
2. 把英文文档翻译成中文文档（帮助有限，官方文档本来就一般般，翻译成中文也不会解决啥问题，有这功夫不如去改官方的英文文档）
3. 做一个简单的资料列表，把一些质量较高的资料整理一下，方便翻阅。

**结论**：
在全部3个解决办法里，我选`方法3`，所以做这个列表。   
并且这里也可以直接放一些我写的总结文章。  

## 如何参与？（添加你认为高价值的资料到列表中）
请创建 Issue 或者直接发送  Pull Request。  

# 列表
* [(英文) 阅读 Contributing 文档](https://github.com/apache/superset/blob/master/CONTRIBUTING.md)：点评：除了官网文档 (指 https://superset.apache.org/docs/intro )应该全部读完之外，最应该读的就是 Contributing 了，因为里面详细介绍了如果要开发的话，如何在本地搭建开发环境。对 Superset 的代码基本情况做了介绍。  

* [(中文) Superset 基本概念](doc/1.Basic-Concept.md): 原创内容，我直接写到 doc 目录里了。 

* [(中文) 书籍《Python+Superset：商业智能数据分析与实战》](https://item.jd.com/10044365591593.html)：我在写这个列表时搜了一下京东，只看到 Superset 有这一本中文图书，改天等我有空看了这本书之后再来写一点评价。  
