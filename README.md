## express-sticky-note-node.js在线备忘录
### 项目介绍
本项目利用express框架搭建的一个node.js在线备忘录网站
利用ejs来书写页面结构、less书写css、Jquery书写js。依据express教程来搭建，设置router来响应请求。将预编译的ejs、less文件转化为HTML、css，使得能够正常运行，利用事件处理中心来进行解耦、瀑布流设计进行排版。另外利用基于Nodejs功能强大的异步ORM框架Sequelize来进行数据管理。在用户登录界面利用OAuth协议，将登录界面转移到github网站上进行登录，其中利用了别人发布的node模块-“passport-github”。购买域名和服务器，将其发布到线上。

#### 功能
- 打开网站
- github登录
- 创建便利贴-有成功提示（操作成功后会按照瀑布流进行排版）
- 修改便利贴（操作成功后会按照瀑布流进行排版）
- 删除便利贴-有删除成功提示（操作成功后会按照瀑布流进行排版）
- 注销账号后，刷新页面会显示所有用户的便利贴，并且便利贴上会有用户名，但是没有权限修改。登录自己的github后，内容只显示自己的。

### 技术栈

HTML、CSS、Jquery、nodejs、webpack、express、less、ejs、OAuth、sequize

### 难点

- express 框架搭建网站的步骤-按照教程一步步引导[express教程](expressjs.com)，经常出错，多调试，确保上一步操作正确，以便寻找问题根源
- less和ejs的使用，直接搜索就会出现相关的教程，要将其变成css和html,不要忘了install相关的模块
- router设置，一定要清楚请求路由的是什么才能正常操作
- 因为涉及到的模块太多了，所以按功能或者按用途进行分类到不同的文件夹中，方便管理，另外就是模块的引用和module.exports不要忘记
- webpack.config 配置

### 线上地址为