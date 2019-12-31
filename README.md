> 这个仓库的Python代码，是我用来从我GitHub上的开源项目仓库中对关注用户进行抽奖的程序。作用是**从一个给定的仓库中爬取点星用户，然后随机抽取N个人的用户名**。
>
> 代码很简单，看注释即可，运行环境`Python3`.

# 何谓福利环节

众所周知，一般我发布的硬件相关的开源项目，都会在项目完成后赠送一些奖品给关注的粉丝如`项目的PCB板`、`开发板`和`元器件`、`一些有意思的工具`、甚至`项目的成品本身`等等。

由于**知乎**平台没有抽奖功能，**Bilibili**的互动抽奖功能以我的粉丝数还不够，所以才准备在本知名同性交友网站上实施抽奖环节。抽奖的细节如下：我的项目开源后都会在GitHub上进行分享和维护，所以大家觉得某个项目有用的话可以参考下图中的指示帮忙点个星星↓

![1577775878470](img/1577775878470.png)



> 当然首先是需要你登陆GitHub账号的，不然我没有办法记录你的ID。

**点过星星的同学会出现在我的项目页列表中↓**



![1577775963868](img/1577775963868.png)



然后我会用本仓库中的程序在这个列表里随机抽取若干账号送出奖品。

抽奖名单出来后我会在知乎和Bilibili发动态公布，然后通过你们在GitHub上的邮箱联系你们，**如果超过一周没有回复邮寄地址的话，那么名额会空出重新抽取（所以请记得更新自己的邮箱噢）**。



# 关于本仓库的抽奖代码

本仓库的代码主要是利用了GitHub的 [REST API v3](https://developer.github.com/v3/)，获取仓库的点星名单。

安装很简单，先用任何方法切换到Python3环境，然后：

```
$ pip install PyGithub
```

再直接运行`GitHubLottery.py`就可以了。

如果大家要自己修改使用的话，把`GitHubLottery.py`里的*仓库名*、*用户名*、*密码*改成自己的就行。

> GitHub为了防止API滥用，对于匿名的请求会限制每个IP地址每个小时只能请求60次；用用户名密码登陆的请求每个小时可以有5000次，因此还是建议大家把代码里的用户名账户给填上。



# 最后也欢迎大家关注我的：

**知乎**@ [稚晖](https://www.zhihu.com/people/zhi-hui-64-54/activities)  （一般在上面更新教程文章）

**Bilibili**@ [稚晖君](https://space.bilibili.com/20259914)  （发布项目视频和日常Vlog）

**GitHub**@ [david-pzh](https://github.com/david-pzh) （项目资料开源和维护地址）

喜欢的话麻烦也顺手给本仓库点个星~

![img](https://pic3.zhimg.com/80/v2-bf913e9c68d5ea7539ad10a2b6b35af2_hd.jpg)