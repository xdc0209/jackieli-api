# 在线习惯-游戏频次

## 描述
> 在线分析-在线习惯-游戏频次

## URL
> [http://192.168.10.117:8080/app/onlineAnalysis/frequencyDailyTable.do](http://dataviewer.ilongyuan.com.cn/app/onlineAnalysis/frequencyDailyTable.do)

## 支持格式
> JSON

## HTTP请求方式
> POST

## 请求参数
> |参数|必选|类型|说明|
|:-----  |:-------|:-----|-----|
|appId    |true    |String(32)|游戏Id |
|platform    |true    |String(32)   |平台 |
|userType  |true     |Integer | 用户类型，1：新增玩家 ，2：活跃玩家|

## 返回字段
> |返回字段|示例|说明            |
|:-----   |:------|:--------    |
|metricName |1499184000000 |游戏次数  |
|percent |'unknown' | 百分比    |
|userNum |2 | 玩家数量   |

## 接口示例
> 地址：[http://192.168.10.117:8080/app/onlineAnalysis/frequencyDailyTable.do](http://dataviewer.ilongyuan.com.cn/app/onlineAnalysis/frequencyDailyTable.do？appId=289ee05803487e57&platform=1&userType=1)
``` javascript
{
    "channelMap": {
        "longyuan5": "longyuan5",
        "jinritt": "jinritt",
        "uctt": "uctt"
    },
    "total": 130,
    "code": 0,
    "data": [
        {
            "metricName":"1",
            "percent":"0.2878381706097669",
            "userNum":"965495"
        }
    ]
}
```

