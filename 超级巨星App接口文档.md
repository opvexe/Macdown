# 超级巨星App接口文档
===========================
## 登录接口
### 1.1 功能描述
<strong>我的界面用户登录</strong>
### 1.2 请求说明
>请求方式: <font color=#0099ff face="黑体"> POST</font><br>
请求URL: <font color=#0099ff face="黑体"> [/user/sendLogin](#)</font><br>

### 1.3 公共请求头参数
```
{
	"token": "1010202933",
	"appkey":"1010202933",
	"uid":"wq11111"
}
```
### 1.4 请求参数
<table>

<tr><td><center>字段</center></td> 
<td><center>字段类型</center></td> 
<td><center>字段说明</center></td> </tr>
<tr>

<tr><td><center>iphone</center></td> 
<td><center>string</center></td> 
<td><center>手机号码</center></td> </tr>
<tr>

<tr><td><center>user_age</center></td> 
<td><center>string</center></td> 
<td><center>用户年龄</center></td> </tr>
<tr>

</table>

```
{
	"iphone": "13437253905",
	"user_age":"18"
}
```

### 1.5 返回参数
```
{
	"ststus": "ok",
	"datas" :  {
				 "uid": "wq11111",
				 "token": "1010202933",
				 "appkey": "1010202933",
				 "user_name": "lisa",
				 "user_perofile": "http:wwww.baidu.com" 
			    }
	"msg": ""
}
```

## 发送验证码接口
### 1.1 功能描述
<strong>发送验证码</strong>
### 1.2 请求说明
>请求方式: <font color=#0099ff face="黑体"> POST</font><br>
请求URL: <font color=#0099ff face="黑体"> [/user/sendCode](#)</font><br>

### 1.3 公共请求头参数
```
{
	"token": "1010202933",
	"appkey":"1010202933",
	"uid":"wq11111"
}
```
### 1.4 请求参数

字段         |字段类型    |字段说明
------------|-----------|-----------
iphone      | string    |手机号码
code        | string    |验证码

### 1.5 返回参数
```
{
	"ststus": "ok",
    "datas": "",
    "msg": ""
}
```
### 错误状态码
参见 [全局响应状态码说明](./接口文档.md/#全局响应状态码说明)


