# 页面路由

## 描述
> 等级分析-页面路由

## URL
> [http://192.168.10.168:8081/app/userLevel/userLevelView.do](http://dataviewer.ilongyuan.com.cn/app/userLevel/userLevelView.do)

## 支持格式
> JSON

## HTTP请求方式
> POST

## 请求参数
> |参数|必选|类型|说明|
|:-----  |:-------|:-----|-----|
|appId    |true    |String|游戏id |    
|platform    |true    |String|平台 |   
|viewName    |true    |String|等级分析 : levelAnalysis |   



## 返回字段
> |返回字段|示例|说明                              |
|:-----   |:----|:-----------------------------    |
|appId      |  3087d9188a0a4e9f  | appId  |
|appName      |  陆战之王  | app名称  |
|platform      |  1  | 平台  |
|platformName      |  Android  | 平台名称  |
|computeEndDate      |  1488729600000，  | 计算结束时间  |
|channelMap      |  "channelMap": {"cn_ios": "cn_ios","asia_ios": "asia_ios",}  | 渠道列表  |

## 接口示例
> 地址：[http://192.168.10.168:8081/app/userLevel/userLevelView.do](http://dataviewer.ilongyuan.com.cn/app/userLevel/userLevelView.do)
``` javascript
{
    {
    "appId": "3087d9188a0a4e9f",
    "appName": "陆战之王",
    "platform": "1",
    "platformName": "Android",
    "computeEndDate": 1488729600000，
    "channelMap": {
        "cn_ios": "cn_ios",
        "asia_ios": "asia_ios",
        "cn_and": "cn_and",
        "ly": "龙渊—安卓",
        "asia_and": "asia_and"
    }
}
```
