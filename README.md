一个用 **go** 编写的阿里云OSS文件访问签名API服务器,用于实现访问控制
***
**TODO**  
- [ ] 签名有效时间  
- [ ] 人机验证  
- [ ] Bucket权限管理  
***
**配置**  
程序在第一次启动时会在目录下生成一个config.json文件,内容如下
```json
{
    "AccessKeyId": "your_access_key",
    "AccessKeySecret": "your_access_secret",
    "port": 1145,
    "sign_time": 40
}
```
将其中的配置替换为你自己的数值.
***
**使用**  
程序会开启一个在设定端口的http服务器