# mybatis-plus代码生成器优化版
基于renren-generator改造   
源开源地址：https://gitee.com/renrenio/renren-generator  
当前实现了：swagger/lombok通过配置开启开启，优化了响应类生成，请通过application.yml和generator.properties配置  
远期目标为：可视化选择连接数据库（或提交sql）、选择是否包含swagger、lombok、用户信息，直接生成下载  
## 改动项：
- 部分配置名称改动（忽略之）
- 优化了生成规则：加入了是否开启swagger是否开启Lombok，但是请注意，如果未开启Lombok，不会生成get和set方法
- 优化了controller的响应：响应类可以自定义，返回方法也可以自定义，如果还不满足，请自行改模板
- 优化了模板格式：加入了swagger相关，并且美化了格式

## 版本：
- 当前实现了：swagger/lombok通过配置开启开启，优化了响应类生成，请通过``application.yml``和``generator.properties``配置
- 远期目标为：可视化选择连接数据库（或提交sql）、选择是否包含swagger、lombok、用户信息，直接生成下载  


## 步骤
（无容器化支持，因为远期目标还没时间搞）  
1. 配置``application.yml``中的数据库地址和数据库类型
2. 配置``generator.properties``中的设置，其中新增部分功能支持都在最后
3. 启动项目，访问``http://127.0.0.1:80``
