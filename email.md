# 验证码服务
发送邮件。该接口都必须携带`signature`参数。


## 接口详情

### 发送邮件
路径：

`GET /email/send`

querystring

参数 | 类型 | 说明
----|------|-----
email|string|用户邮箱
subject|string|邮件主题
content|string|邮件正文
signature|string|签名


demo:

http://micro-service.demo.tsq.me/email/send?signature=561ED961&email=i@tsq.me&subject=test&content=hello

成功返回：


```json
{
  "success": true
}
```

失败返回：

```json
{
  "success": false,
  "msg": "signature is invalid, please contact manager"
}
```
