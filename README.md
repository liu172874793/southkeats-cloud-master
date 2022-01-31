## 平台简介

### 文档 http://doc.southkeats.com 
### 启动演示视频 https://www.bilibili.com/video/southkeats/

### 源码
- [Github](https://github.com/liu172874793/southkeats-cloud-master.git)
- [Gitee](https://gitee.com/liu172874793/southkeats-cloud-master.git)

#### 友情链接 [南慈/SouthKeats-Cloud](https://github.com/liu172874793/southkeats-cloud-master.git) Element UI版本。
#### 分支说明

- **master** spring原生方式，使用eureka做注册中心和spring config做配置中心
- **nacos** 集成spring-cloud-alibaba 使用nacos做注册中心和配置中心

本项目FORK自  [南慈/SouthKeats](https://github.com/liu172874793/southkeats-cloud-master.git)

蓝本是[zhangmrit/Southkeats](https://github.com/liu172874793/southkeats-cloud-master.git)

依次绑定host：

127.0.0.1 eureka7001.com

127.0.0.1 gateway.com

如果要使用eureka集群，请依次绑定eureka7002.com,eureka7003.com后修改各项目中的注释部分

```
southkeats-cloud
|
├──southkeats-common --通用包
|  |
|  ├──southkeats-common-core --核心工具包
|  |
|  ├──southkeats-common-redis --redis工具包
|  |
|  ├──southkeats-common-log --日志工具包
|  |
|  ├──southkeats-common-auth --权限工具包
|
├──southkeats-config --cloud统一配置中心
|
├──southkeats-eureka --注册中心
|
├──southkeats-gateway --网关
|
├──southkeats-service-api --服务api模块
|  |
|  ├──southkeats-system-api --系统业务api
|
├──southkeats-service --微服务
|  |
|  ├──southkeats-system --系统业务
|  |
|  ├──southkeats-auth --授权中心
|  |
|  ├──southkeats-gen --代码生成
|  |
|  ├──southkeats-dfs --文件
|
├──southkeats-tool --工具
|  |
|  ├──southkeats-monitor --监控中心
|
├──southkeats-ant --前端 使用ant design框架

```



启动顺序：
- eureka
- config
- gateway
- system
- auth
- gen 可选
- dfs 可选

菜单sql有增加字段，以上传到sql文件
该分支是ant分支，前端使用ant-design-vue 项目地址 [southkeats-ant](https://github.com/liu172874793/southkeats-ant-master.git)

monitor使用springadmin完成,目前只是最简单的用法,[详戳](http://southkeats.com/#/extra?id=%e7%9b%91%e6%8e%a7)

## SouthKeats Cloud交流群

QQ群：869292399

### 鸣谢
- [南慈](https://gitee.com/y_project/SouthKeats) 开源框架，以及演示服务器提供
- [antdv-pro](https://github.com/vueComponent/ant-design-vue-pro) 前端集成框架
- [AJ-Captcha](https://gitee.com/anji-plus/captcha) 滑动验证码

欢迎pr或者加入，给个star是最好的鞭策

