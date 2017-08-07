# 微服务
提供一系列API用于辅助API Server

API请求域名是： `http://micro-service.demo.tsq.me`
 
项目地址为: https://github.com/tsq-nodejs/micro-service

## 现有服务

* [发送邮件](./email.md): 发送邮件到用户邮箱
* [发送验证码](./sms.md): 发送验证码到用户手机
* 文件上传: 上传文件至阿里云OSS

## 关于signature
某些API在使用时，需要在url后面加上`signature`这条querysting， `signature`可在[micro-service项目](https://github.com/tsq-nodejs/micro-service/blob/master/routes/whitelist.json)中进行自定义配置。其实际为一个白名单
列表，只接受来自白名单内signature的请求，防止被他人随意调用。


## 本地运行本项目

```shell
git clone git@github.com:tsq-nodejs/document.git
cd document
npm i -g gitbook-cli
gitbook install
npm start 
```
