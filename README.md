<p align="center">
  <a href="https://github.com/Jnu-Survey">
    <img src="https://raw.githubusercontent.com/Jnu-Survey/Introduce/main/assets/logo.png" width="200" height="200" alt="logo">
  </a>
</p>
<div align="center">

# Jnu-Survey-Data

_✨ 由暨南大学某软件工程课程小组维护 ✨_  

</div>

<p align="center">
  <a href="https://github.com/HengY1Sky/JNU-ToolsBox">
    <img src="https://img.shields.io/badge/Version-0.0.1-orange" alt="license">
  </a>
</p>

##  项目介绍：

![概念图](https://raw.githubusercontent.com/Jnu-Survey/Introduce/main/assets/poster_1.png)

暂时借助面向软件工程大作业编程的契机，做一个**在线调查问卷管理系统**。

相比较于市面上的收费管理软件，我们的目标是：**在满足基础的功能下，基础版源码开源**

方便各位大佬面向需求进行**二次开发**～ （您的一个个star✨是对我们的认可）

🔭：**如果想知道对应的代码如何实现/亮点等，请到对应的仓库下进行查看**

- 前端开源地址：https://github.com/Jnu-Survey/WeChatFrontEnd
- 后端开源地址：https://github.com/Jnu-Survey/GinBackEnd
- 状态吗返回文档：https://github.com/Jnu-Survey/Introduce/blob/main/code.md
- APIfox在线文档地址：https://www.apifox.cn/apidoc/shared-1a5c59a5-a923-47a7-8dac-a03c3e7b7577

> 后期可能会根据学校需求做定制化的商业版，商业版不涉及隐私的都会拿过来进行更新。

##  技术栈：

###  前端：

- 主语言：Css、JavaScript、Typescript

- 开发框架：微信小程序框架（App Service和View）

- 使用组件库：Vant-Weapp、Animate、echarts

- 代码规范：ESLint、Prettier

- 其他：Websocket、虚拟列表

###  后端：

- 主语言：Goalng

- 开发框架：Gin

- 数据库：Mysql、MongoDB

- 中间件：Redis、RabbitMq

- 对象存储：七牛云对象存储

- 其他：压缩算法[ZSTD](https://github.com/klauspost/compress/tree/master/zstd)；WebSocket；布隆过滤器

###  部署：

- WEB服务：Nginx

- 环境编排：Docker-Compose

- CDN加速：七牛云CDN

###  其他：

- Sketch（仅面向Mac用户）

- MasterGo

- 蓝湖插件

- Apifox

## 职能分配

- [HengY1Coding✨](https://github.com/orgs/Jnu-Survey/people/HengY1Sky)：产品设计；UI设计；后端研发；测试
- [MMMMMMaxuan](https://github.com/orgs/Jnu-Survey/people/MMMMMMaxuan)：前端研发
- [BatchClayderman](https://github.com/orgs/Jnu-Survey/people/BatchClayderman)：产品报告；PPT汇报
- [chenccc0127](https://github.com/orgs/Jnu-Survey/people/chenccc0127)：产品报告；PPT汇报

##  项目定位

![项目定位](https://raw.githubusercontent.com/Jnu-Survey/Introduce/main/assets/location_1.png)

##  整体架构

![架构图](https://raw.githubusercontent.com/Jnu-Survey/Introduce/main/assets/framework.png)

##  性能测试

![性能测试](https://raw.githubusercontent.com/Jnu-Survey/Introduce/main/assets/performance_1.png)

##  未来展望/更新日志

- B端研发暂时没写：等后面我(HengY1Coding)自己写上去
- 表格的生成与导出等操作：方便第三方分析
- 上升为商家版本：暂时为个人开发小程序，部分微信小程序功能被阉割

当前版本为：1.0
由于前端同学的经验仍然欠缺以及我忘记提醒了，导致没写全局的请求。在正式发布后出现了几个问题，因为是个人版小程序不符合微信小程序审核，导致我们没法多次提交正式版本。

- 如果你是参与者；第一次进入小程序Token没有则会打不开表单；而需要到小程序里面进行登陆后才能正常使用
- 如果你已经提交了，没有提示你说无法再次提交，这就是没写全局的问题（后端的返回码是完成了的）
- 分析表单功能，感觉第三方不太兼容，需要多次打开才能看见，前面都是空白的
- Websocket的断开与连接问题，如果填表记录断开且重连接，前端忘记清理已经存在了的；会导致"重复"
- 如果你在分享的表单里面登陆后；再次主动进入小程序，个人中心已经登陆但是登陆状态仍然是未登陆

以上造成不好体验十分抱歉；我们会在随后进行改进

<details>
<summary>20220525</summary>
<h3>杀青</h3>

- 经过测试后返现返回顺序反了；影响体验
- Websocket发现Bug并且联合在此再次测试了下
- 前端测试完毕
- 经过测压后发现：如果单纯的链接的话会导致链接失败；所以加入连接池
- 后端经过脱敏后正式开源
</details>

##  安全审计/修复日志

**后端为Golang语言**，欢迎相关技术大佬进行**代码审计**。

**发现安全问题奖励20-200元不等**，可以直接提交ISSUE/直接联系我。我自掏腰包🐶

我(HengY1Coding)的联系方式在我的个人主页：https://github.com/HengY1Sky/
