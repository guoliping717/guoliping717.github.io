
---
title: Hexo 博客终极玩法：语雀-云端写作，自动部署Github
date: 2019-01-23 22:48:55 +0800
tags: [Hexo]
categories: 前端
---
Hexo + Github + 语雀 + yuque-hexo +travis-ci+severless 打造全自动持续集成个人博客，云端写作，自动部署，完美体验~
### 一、Hexo+Github 的痛点
#### 1.为啥要用hexo+github？
作为一个程序猿，博客肯定是必须要有的拉，github也是必须要混的拉~所以:
* hexo + github = 高大上

![image.jpeg](https://cdn.nlark.com/yuque/0/2019/jpeg/155457/1546857679810-d82e3d46-e960-419c-a715-0a82c48a2fd6.jpeg#align=left&display=inline&height=225&linkTarget=_blank&name=image.jpeg&originHeight=225&originWidth=225&size=6267&width=225)
#### 2.蛋疼的写作体验
使用hexo，会面临如下问题：
* 博客源码怎么管理？
* 图片存在哪？
* 如何编写markdown文件？

相信很多人都在使用本地编辑器来写博客，那体验，真心蛋疼，比如说vscode，可视化插件一般般，图片还不能复制黏贴，想插入个图片还要先保存成文件放在本地，然后再引用，啥？你说七牛云存储？哪有复制黏贴爽呀~<br />当然，博客源码可以使用travis-ci 来做持续集成，想写博客或者换个电脑，clone一下源仓库，写完push一下，就可以不用管了。but，比起独立站点的博客，如wordpress，还是觉得写作体验有点不爽。<br />![image.jpeg](https://cdn.nlark.com/yuque/0/2019/jpeg/155457/1546858156666-f3f7ae20-c7f8-49b9-849d-b4364f3685f7.jpeg#align=left&display=inline&height=213&linkTarget=_blank&name=image.jpeg&originHeight=213&originWidth=237&size=5810&width=237)
#### 3. 脑洞大开：
偶然间，朋友安利了语雀这个文档写作平台，觉得这就是完美的写作体验，各种UI和编辑器都很舒服~秀个图：<br />![image.png](https://cdn.nlark.com/yuque/0/2019/png/155457/1546858295510-9ca72eb5-b3ae-4d7c-8478-d8d1cda959d0.png#align=left&display=inline&height=821&linkTarget=_blank&name=image.png&originHeight=903&originWidth=1789&size=119669&width=1626)

markdown编辑器也是巨爽：<br />![image.png](https://cdn.nlark.com/yuque/0/2019/png/155457/1546858354478-127bd82a-7958-40ce-b760-07e469bd55ba.png#align=left&display=inline&height=840&linkTarget=_blank&name=image.png&originHeight=924&originWidth=1890&size=125288&width=1718)

于是乎，就在想能不能在语雀里写作，写完之后自动同步到Github的博客呢？年轻就要有激情，说干就干，花了一天时间，结合了yuque-hexo、travis-ci、Github-pages之后，终于跑通了整个写作、发布、自动部署的流程~<br />![image.jpeg](https://cdn.nlark.com/yuque/0/2019/jpeg/155457/1546858544992-c921de6f-b08a-469a-bd5f-81996309443b.jpeg#align=left&display=inline&height=225&linkTarget=_blank&name=image.jpeg&originHeight=225&originWidth=225&size=10511&width=225)


