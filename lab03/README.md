实验3:Apollo Client和Spring集成(XML方式)
======

### 一、实验步骤

#### 1. 启动配置中心服务
参考[实验1](../lab01)

**注意清理前面实验的本地缓存**

#### 2. 环境和配置中心地址
环境变量方式

```
-Denv=dev
-Ddev_meta=http://localhost:8080
```

#### 3. spring.xml配置

注意点：
  * xmlns:apollo声明
  * apollo:config顺序
  * 配置缺省值

#### 4. 配置更新

缺省名字空间下的timeout

#### 5. 配置重载

TEST1.apollo名字空间下的batch配置


### 二、参考

1. 代码[XmlApplication](https://github.com/ctripcorp/apollo/blob/master/apollo-demo/src/main/java/com/ctrip/framework/apollo/demo/spring/xmlConfigDemo/XmlApplication.java)
2. 文档[Java客户端使用指南](https://github.com/ctripcorp/apollo/wiki/Java%E5%AE%A2%E6%88%B7%E7%AB%AF%E4%BD%BF%E7%94%A8%E6%8C%87%E5%8D%97)




