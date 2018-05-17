实验5:Apollo Client和Spring Boot集成
======

### 一、实验步骤

#### 1~6. 同实验4

Spring Boot有一些场景需要配置在更早的阶段注入

* 使用@ConditionalOnProperty的场景
* 是有一些spring-boot-starter在启动阶段就需要读取配置做一些事情（如spring-boot-starter-dubbo)


启动方式：
```
// 启动
apollo.bootstrap.enabled=true
// 注入多个名字空间
apollo.bootstrap.namespaces = application,TEST1.apollo
```

#### 7. 条件属性(ConditionalOnProperty)

@ConfigurationProperties如果需要在Apollo配置变化时自动更新注入的值，需要配合Spring Cloud的RefreshScope使用

* Annotation
```
// 条件属性
@ConditionalOnProperty
// 自动刷新
@RefreshScope
// 监听Apollo事件
@ApolloConfigChangeListener
```


### 二、参考

1. 代码[SpringBootSampleApplication](https://github.com/ctripcorp/apollo/blob/master/apollo-demo/src/main/java/com/ctrip/framework/apollo/demo/spring/springBootDemo/SpringBootSampleApplication.java)
2. 文档[Java客户端使用指南](https://github.com/ctripcorp/apollo/wiki/Java%E5%AE%A2%E6%88%B7%E7%AB%AF%E4%BD%BF%E7%94%A8%E6%8C%87%E5%8D%97)




