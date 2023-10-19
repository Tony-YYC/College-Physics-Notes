---
title: 博客搭建与基础配置
tags: 1
categories: 1
---
第一次尝试搭建个人博客。
本博客使用[b站教程](https://www.bilibili.com/video/BV1ts4y1f7Gu)，[hexo](https://hexo.io/zh-cn/index.html)开源项目，以及[ayer](https://shen-yu.gitee.io/2019/ayer/)主题。
具体流程：下载[git](https://git-scm.com/)，[node.js](https://nodejs.org/zh-cn/)
<!--more-->

### 1.git、hexo、node.js环境搭建
下载[git](https://git-scm.com/)，[Node.js](https://nodejs.org/zh-cn/)。
git下载完毕后，在cmd窗口中输入```node-v```查看版本号，如果出现版本号，则说明安装成功。
新建一个下载hexo的文件夹，进入后右键选择git bash打开git窗口，分别输入[hexo官网](https://hexo.io/zh-cn/index.html)的命令。
```
# 1下载
npm install hexo-cli -g 
# 2初始化博客，运行完毕会出现blog文件夹
hexo init blog
# 3进入博客
cd blog
# 4下载 
npm install
# 5运行博客（为原始版本、默认主题，之后可以下载其他主题）
hexo server 
```


### 2.hexo与hexo主题下载
[hexo](https://hexo.io/zh-cn/index.html)，[ayer](https://shen-yu.gitee.io/2019/ayer/)主题。



### 3.配置
根据需求，修改`config.yml`与`config.ayer.yml`中的具体配置
`config.ayer.yml`中可以修改网页封面、公告栏、鼠标样式、广告图标、友情链接
注意，`config.yml`与`config.ayer.yml`中冒号“：”后均需要加空格，否则报错

### 4.Tips
```
hexo clean 
```
清除缓存(public文件夹)能解决大部分无法更新的问题。
也因此，请不要把重要的文件存在public文件夹下。

### 5.具体配置与插件
详见下一篇文章。

### 6.将静态网页放在gitee pages上
详见[b站教程](https://www.bilibili.com/video/BV1ts4y1f7Gu)
23333


<details>
<summary>2333</summary>

23333

</details>


















