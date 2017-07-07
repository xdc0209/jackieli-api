# 滚服设备路由

## 描述
> 用户分析-滚服设备路由


## URL
>[http://192.168.10.111:8080/app/rollDevAnalysis/rollUserView.do?](http://192.168.10.111:8080/app/rollUserAnalysis/rollUserView.do?)

## 支持格式
>JSON

## HTTP请求方式
>POST

## 请求参数
>|参数|必选|类型|说明|
|:------|:-----|:----|:-----|
|appId    |true|String(32)|游戏Id|
|platform|true|String(32)|平台|
|viewName|true|String(32)|滚服玩家视图：rollDevView|

## 返回字段
>|返回字段|说明|示例|
|:-----|:----|:----|
|appId|游戏Id|3087d9188a0a4e9f|
|appName|游戏名称|陆战之王|
|platform|平台|1|
|platformName|平台名称||
|channelMap|渠道列表|"channelMap": {"cn_ios": "cn_ios","asia_ios": "asia_ios",}|

## 接口示例
>地址：[http://192.168.10.111:8080/app/rollDevAnalysis/rollUserView.do?](http://192.168.10.111:8080/app/rollDevAnalysis/rollUserView.do?)
``` javascript
{
       "appId": "3087d9188a0a4e9f",
       "appName": "陆战之王",
       "platform": "1",
       "platformName": "Android",
       "channelMap": {
           "cn_ios": "cn_ios",
           "asia_ios": "asia_ios",
           "cn_and": "cn_and",
           "ly": "龙渊—安卓",
           "asia_and": "asia_and"
       }
}  
```
