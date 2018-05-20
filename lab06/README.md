实验6:Apollo开放平台接入实操（Lab6）
======

### 一、实验步骤

#### 1. 注册第三方应用

```
http://{portal_address}/open/manage.html
```

#### 2. 给第三方应用授权

绑定App或Namespace

#### 3. 调用Http REST接口

* Http Header 1
  * Authorization
  * token
* Http Header 2
  * Content-Type
  * application/json;charset=UTF-8

#### 4. 获取App环境，集群信息

- URL : http://{portal_address}/openapi/v1/apps/{appId}/envclusters
- Method : GET
- Request Params : 无

#### 5. 获取集群下所有Namespace信息接口

- URL : http://{portal_address}/openapi/v1/envs/{env}/apps/{appId}/clusters/{clusterName}/namespaces
- Method: GET
- Request Params: 无

#### 6. 获取某个Namespace信息接口

URL ： http://{portal_address}/openapi/v1/envs/{env}/apps/{appId}/clusters/{clusterName}/namespaces/{namespaceName}
Method ： GET
Request Params ：无

#### 7. 其它操作结构

1.  创建Namespace
2.  获取某个Namespace当前编辑人接口
3.  新增配置接口
4.  修改配置接口
5.  删除配置接口
6.  发布配置接口
7.  获取某个Namespace当前生效的已发布配置接口

### 二、参考

1. 文档[Apollo开放平台](https://github.com/ctripcorp/apollo/wiki/Apollo%E5%BC%80%E6%94%BE%E5%B9%B3%E5%8F%B0)




