# 验证码服务
发送验证码。该接口都必须携带`signature`参数。


## 接口详情

### 发送验证码
路径：

`GET /sms/send`

querystring

参数 | 类型 | 说明
----|------|-----
phone|string|用户手机号
signature|string|签名


demo:

http://micro-service.demo.tsq.me/sms/send?signature=561ED961&phone=17705143392

成功返回：


```json
{
  "success": true,
  "code": "1990"
}
```

失败返回：

```json
{
  "success": false,
  "msg": "signature is invalid, please contact manager"
}
```
