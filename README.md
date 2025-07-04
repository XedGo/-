# 抖音直播防护墙

#### 介绍
主要用于AI无人直播、直播间有大量捣乱的人。当然每个人都能用

可以基于用户以下信息进行拉黑、警告：
- 昵称
- 签名
- 性别
- 弹幕
- 进入直播间方式
- 分享直播间
- 省份
- 城市
- 关注量
- 粉丝量
- 是否开通过橱窗
- 是否开通过直播带货
- 是否开通过视频带货
- 用户等级

![image](https://github.com/user-attachments/assets/6e2b7d69-4522-4f36-a9e4-9748513c80cf)



#### 原理及安全性

 **原理** 
- 通过监听弹幕实时判断是否违规
- 通过抓包的API实时提取用户信息
- 通过自动化操作浏览器实现获取cookie

 **安全** 
本应用会获取直播间管理员cookie进行操作。如果不放心，你可以禁止软件联网，但是必须放行下面几个域名：
- live.douyin.com 【抖音接口】
- www.douyin.com 【抖音接口】
- webcast100-ws-web-lq.douyin.com 【抖音接口】
- webcast5-ws-web-lq.douyin.com 【抖音接口】
- registry.npmmirror.com 【阿里NPM源（用于安装chrome或者edge驱动）】
- rap2api.taobao.org 【淘宝mock接口，用于检测更新，如果不需要检测更新可以屏蔽】

下载：https://github.com/XedGo/douyin-safe-dun/releases

