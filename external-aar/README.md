# GLSDK
GrabLink-SDK

## SDK开发模式

设置建议直接依赖各个module，方便源码修改后直接生效。依赖module包括：

```gralde
    api project(":ExternalAAR")
```

## 发布到jcenter时
* 上传新版时版本名称必须改变，否则无法上传
* 修改module中build.gradle中的 version = "x.x.x"


> 构建命令
```
   //install
   ./gradlew :ExternalAAR:clean :ExternalAAR:install

   //上传到jcenter
   ./gradlew :ExternalAAR:bintrayUpload
```

> 上传用户和KEY

```
账户: everonetxl
KEY: 请自行到bintray用户信息中自行获取
```