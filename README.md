

# 目录结构说明

目前的目录结构和以往目录结构有说区别
>* 以往的项目分为DAO-Service-controller.
>* 本项目目录结构 Repository - Service - Facade -Controller
目的是希望同一个项目结构。使用多个架构实现。单项目、maven项目、dubbo项目、spring cload、变化持久成实现为mybatis

```

├── resources                  资源配置文件
│   ├──messages...             国际化
│   ├──applicationContext.xml  配置包括jpa-data、国际化等
│   ├──log4j.properties        日志配置
│   ├──config.properties       配置项
│   ├──spring-mvc.xml          SpringMVC配置
├── webapp
│   ├── WEB-INF                          
│   │   │
│   │   └── web.xml   
├── src.rjsoft
│   │
│   ├── uums                   统一用户管理
│   │   ├── api                api\controller
│   │   ├── core               dao\server
│   │   ├── facade             facade
│   ├── common                 
│   │   ├── entity             基础实体类
│   │   ├── exception          异常基类
│   │   ├── modal              与JpaSearch相关
│   │   ├── repository         对Jpa封装
│   │   ├── service            Service基类
│   │   ├── utils              工具类
│   │   │   ├── security               安全md5加密
│   │   │   ├── validate               数据合法性验证 
│   │   │   ├── DateUtil.java          时间工具类 
│   │   │   ├── MessageUtils.java      国际化工具类 
│   │   │   ├── NetworkUtil.java       获取ip\浏览器信息等
│   │   │   ├── SpringUtils.java       获取实例
│   │   │
│   │   └── vo                 VO基类
│   │
└── pom.xml                    maven pom 包依赖
```

