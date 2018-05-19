实验1:Apollo快速起步
======

### 一、实验步骤

#### 1. 下载Quick Start安装包

下载[apollo-build-scripts](https://github.com/nobodyiam/apollo-build-scripts)项目

#### 2. 创建数据库

创建[ApolloPortalDB](https://github.com/nobodyiam/apollo-build-scripts/blob/master/sql/apolloportaldb.sql)

校验App表

创建[ApolloConfigDB](https://github.com/nobodyiam/apollo-build-scripts/blob/master/sql/apolloconfigdb.sql)

校验Item表

#### 3. 更新数据库连接信息

demo.sh里头用户名/密码

#### 4. 启动Apollo配置中心
确保8070/8080/8090端口未被占用
```
./demo.sh start
```

#### 5. 登录Apollo

```
超级用户apollo/admin
```

#### 6. 测试客户代码
运行客户端
```
./demo.sh client
```

#### 7. 修改和发布配置

#### 8. 创建新用户和项目

用户管理
```
http://{portal地址}/user-manage.html 
```
应用配置
```
client/META-INF/app.properties
```

### 二、参考

1. 代码[SimpleApolloConfigDemo](https://github.com/ctripcorp/apollo/blob/master/apollo-demo/src/main/java/com/ctrip/framework/apollo/demo/api/SimpleApolloConfigDemo.java)
2. 文档[Quick Start](https://github.com/ctripcorp/apollo/wiki/Quick-Start)




