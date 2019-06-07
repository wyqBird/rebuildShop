# Dubbo、SpringBoot 重构淘淘商城

## 一、所用工具

- 开发工具：IDEA、Maven
- 前端页面：JSP、JQuery、CSS、javascript
- 后端服务：SpringBoot、MyBatis、Druid、MySQL
- 中间件：Dubbo、Redis、Zookeeper、ElasticSearch、ActiveMQ
- 版本管理：git

原来使用的是Spring、SpringMVC、MyBatis，没有dubbo，且搜索使用的是Solr。

## 二、商城系统架构(基于SOA)

1、SOA简介

SOA：Service Oriented Architecture面向服务的架构。也就是把工程拆分成服务层、表现层两个工程。服务层中包含业务逻辑，只需要对外提供服务即可。表现层只需要处理和页面的交互，业务逻辑都是调用服务层的服务来实现。

![淘淘商城系统架构](G:\自己的项目\淘淘商城\淘淘商城系统架构.png)

## 三、现有功能

1、用户注册、登陆、退出

2、主页面大广告位的显示、商品类别的显示

3、商品搜索、查看详情、加入购物车、生成订单

4、后台商品增删改查、商品内容增删改查、将数据库数据导入索引库

## 四、技术点详解

1、工程搭建和启动

2、SpringBoot2 整合 JSP

3、单点登陆

4、Solr 和 ElasticSearch

5、PageHelper 的使用

6、图片服务器 FastDFS

7、富文本编辑器

8、浏览器兼容性问题

9、缓存一致性问题

10、全局异常处理

11、网页静态化

12、Jsonp

13、自定义登陆拦截器