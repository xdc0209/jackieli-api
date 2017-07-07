# 活跃玩家

## 描述
> 用户分析-活跃玩家-活跃玩家

## URL
> [http://192.168.10.117:8080/app/userAnalysis/selectActiveUserTable.do](http://dataviewer.ilongyuan.com.cn/app/userAnalysis/selectActiveUserTable.do)

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
|:-----   |:------|:--------    |
|dt |1499184000000 |时间  |
|addActiveUserNum |2 | 新增玩家        |
|dailyActiveUserNum |2|DAU |
|exceptPayActiveUserNum |2|非付费玩家 |
|monthlyActiveUserNum |2|月度活跃玩家 |
|weeklyActiveUserNum |2|每周活跃玩家 |
|dailyActiveUserNum |2|日活跃玩家 |
|dauMauRatio |0.11754587155963303| 可体现用户的总体粘度，此比例越趋近于1，代表月活跃中有更多用户多日活跃；比例越趋近0，则代表大量用户只在一日中活跃。|

## 接口示例
> 地址：[http://192.168.10.117:8080/app/userAnalysis/selectActiveUserTable.do](http://dataviewer.ilongyuan.com.cn/app/userAnalysis/selectActiveUserTable.do？appId=289ee05803487e57&platform=1)
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
            "addActiveUserNum":2,
            "dailyActiveUserNum":1230,
            "dt":1499184000000,
            "exceptPayActiveUserNum":1225,
            "payActiveUserNum":5,
            "monthlyActiveUserNum":17456,
            "weeklyActiveUserNum":14566,
            "dailyActiveUserNum":12548,
            "dauMauRatio":0.11754587155963303
        }
    ]
}
```