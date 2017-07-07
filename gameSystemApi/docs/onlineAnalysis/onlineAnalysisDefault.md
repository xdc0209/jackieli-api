# 在线习惯页面路由

## 描述
> 在线分析-在线习惯页面路由

## URL
> [http://192.168.10.117:8080/app/onlineAnalysis/onlineAnalysisDefault.do](http://dataviewer.ilongyuan.com.cn/app/onlineAnalysis/onlineAnalysisDefault.do)

## 支持格式
> JSON

## HTTP请求方式
> POST

## 请求参数
> |参数|必选|类型|说明|
|:-----  |:-------|:-----|-----|
|appId    |true    |String(32)|游戏Id |
|platform    |true    |String(32)   |平台 |


## 返回字段
> |返回字段|示例|说明|
|:-----|:----|:----|
|appId|游戏Id|3087d9188a0a4e9f|
|appName|游戏名称|陆战之王|
|platform|平台|1|
|platformName|平台名称|
|computeEndDate|1488729600000|当前已计算的时间点|

## 接口示例
> 地址：[http://192.168.10.117:8080/app/onlineAnalysis/onlineAnalysisDefault.do](http://dataviewer.ilongyuan.com.cn/app/onlineAnalysis/onlineAnalysisDefault.do？appId=289ee05803487e57&platform=1)
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