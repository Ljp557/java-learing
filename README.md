| 技术                   | 版本    | 说明             |
| ---------------------- | ------- | ---------------- |
| SpringBoot             | 2.3.0   | 容器+MVC框架     |
| SpringSecurity         | 5.3.2   | 认证和授权框架   |
| MyBatis                | 3.5.4   | ORM框架          |
| MyBatis-Plus           | 3.3.2   | MyBatis增强工具  |
| MyBatis-Plus Generator | 3.3.2   | 数据层代码生成器 |
| Redis                  | 5.0     | 分布式缓存       |
| Docker                 | 18.09.0 | 应用容器引擎     |
| Druid                  | 1.1.10  | 数据库连接池     |
| JWT                    | 0.9.0   | JWT登录支持      |
| Lombok                 | 1.18.12 | 简化对象封装工具 |


docker安装最常用的MySql和Redis服务即可,数据库中需要导入`mall_tiny.sql`脚本。


src
├── common -- 用于存放通用代码
|   ├── api -- 通用结果集封装类
|   ├── config -- 通用配置类
|   ├── domain -- 通用封装对象
|   ├── exception -- 全局异常处理相关类
|   └── service -- 通用业务类
├── config -- SpringBoot中的Java配置
├── domain -- 共用封装对象
├── generator -- MyBatis-Plus代码生成器
├── modules -- 存放业务代码的基础包
|   └── ums -- 权限管理模块业务代码
|       ├── controller -- 该模块相关接口
|       ├── dto -- 该模块数据传输封装对象
|       ├── mapper -- 该模块相关Mapper接口
|       ├── model -- 该模块相关实体类
|       └── service -- 该模块相关业务处理类
└── security -- SpringSecurity认证授权相关代码
    ├── annotation -- 相关注解
    ├── aspect -- 相关切面
    ├── component -- 认证授权相关组件
    ├── config -- 相关配置
    └── util -- 相关工具类
```

