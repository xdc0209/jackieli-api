

# 报表分析-报表数据明细-页面路由

##描述
> 报表分析-报表数据明细-页面路由

## URL
> [http://192.168.10.117:8080/app/report/toReportDataDetail.do](http://dataviewer.ilongyuan.com.cn/app/report/toReportDataDetail.do)

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
> |返回字段|示例|说明            |
|:-----|:----|:----|
|appId|3087d9188a0a4e9f|游戏Id|
|appName|陆战之王|游戏名称|
|platform|1|平台|
|platformName||平台名称|
|computeEndDate|1488729600000|当前已计算的时间点| 
|channelMap|1488729600000|当前已计算的时间点| 
|commonReportConfig|CommonReportConfig对象："CommonReportConfig{" + "id=" + id + ", userId=" + userId + ", appId=" + appId + ", platform='" + platform + '\'' + ", reportType='" + reportType + '\''+ ", emailList='" + emailList + '\'' + ", postTime='" + postTime + '\'' + ", channelList='" + channelList + '\'' + ", metricCollection='" + metricCollection + '\'' + ", isSubscribe='" + isSubscribe + '\'' + ", gmtCreate=" + gmtCreate + ", gmtModify=" + gmtModify + '}';|报表配置| 

## 接口示例
> 地址：[http://192.168.10.117:8080/app/report/toReportDataDetail.do](http://dataviewer.ilongyuan.com.cn/app/report/toReportDataDetail.do？appId=289ee05803487e57&platform=1)
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