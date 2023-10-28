---
layout:     post
title:      天地框架
subtitle:   天地框架，QQ机器人
date:       2022-10-2
author:     无名
header-img: img/hs.jpg
catalog: 	 true
tags:
    - 框架
    - 开发技巧
---
## 提示
本介绍为2022年所写gocqhttp开发者已未维护请各位另寻他路
## 框架
QQ框架没什么新意
接下来用10分钟左右时间理解
你也能做出属于你自己的QQ框架
依据[gocqhttp](https://docs.go-cqhttp.org)为核心
其实就是监视gocqhttp反馈post值然后给插件然后访问内网api
发送消息 个人认为（没什么厉害的）
[栗子（密码：tdkj）](https://pan.laorubin.cn/s/knquQ)用于接受json原文本消息
接收后json解析，提取，调用就行了（作者建议用dll以防被破解）
api看一看官方文档就懂了
其实也没什么可讲的就是gocqhttp监视，调用。
不懂得加QQ:3107856775(花小钱提问)
## 开发者dll调用
复制文件到一个地址

dll调用这个地址的固定文件就欧克了

这里建议关闭框架官方dll删除

开启框架：安装dll

确保源码的安全性（懂得都懂）

可以使用易语言来写也可以用python等多种语言来写无所谓

能跑就行对不对😁😁😁😁

### 监视自定义
自定义监视端口可以让同一网络下多开（比较方便）

配置文件：config.yml

http post（记得注释删除以免无法使用）

更改端口就行了（当txt文件读就行了然后转一下编码格式就行了）

### 形式
gocqhttp：属于客户端

用编程软件写个服务端接口与gocqhttp的yml配置文件相（端口）同即可

然后接受消息（返回数据）json消息（解析即可）

### api
API格式是：发送群消息：http:// + yml设置ip + yml设置端口 + /send_group_msg?group_id=” ＋ 发送群号 ＋ “&message=” ＋ 发送内容

注意：中文要转为utf8格式（否则发送消息会出现乱码）

换行符：%0a（直接用浏览器访问用这个易语言也用这个）

易语言：有些东西需要手动转义比如换行符，xml，json（建议使用”子文本替换“（可以减少麻烦））
## cmd管道
这个命令（cmd /C cmd /K tdkj-http.exe >"C:\1.txt"）生成but文件覆盖

然后进行编码转换读取就行了

可以用于登入
## 结尾
转载请注原创（跪谢）
