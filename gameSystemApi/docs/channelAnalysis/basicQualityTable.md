# 渠道分析-质量指标总览

##描述
> 渠道分析-质量指标总览

## URL
> [http://192.168.10.117:8080/app/channelAnalysis/basicQualityTable.do](http://dataviewer.ilongyuan.com.cn/app/channelAnalysis/basicQualityTable.do)

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
|avg1DayRetentionNum |0 |平均次日留存人数  |
|avg3DayRetentionNum | 0| 平均3日留存人数    |
|avg7DayRetentionNum |0 | 平均7日留存人数    |
|avgDailyActiveUserNum |0 | 平均日活跃数   |
|avgDailyActiveUserRatio |1 | 平均日活跃率   |
|channel |"amoby" | 渠道   |
|detail |"app/channelAnalysis/channelQuality.do?appId=289ee05803487e57&platform=1&channel=amoby" | 详细   |
|firstWeekPayRatio |1 | 玩家转化率   |

## 接口示例
> 地址：[http://192.168.10.117:8080/app/channelAnalysis/basicQualityTable.do](http://dataviewer.ilongyuan.com.cn/app/channelAnalysis/basicQualityTable.do？appId=289ee05803487e57&platform=1&userType=1)
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
            "avg1DayRetentionNum":0,
            "avg3DayRetentionNum":0,
            "avg7DayRetentionNum":0,
            "avgDailyActiveUserNum":0,
            "avgDailyActiveUserRatio":1,
            "channel":"amoby",
            "detail":"app/channelAnalysis/channelQuality.do?appId=289ee05803487e57&platform=1&channel=amoby",
            "firstWeekPayRatio":0
        }
    ]
}
```

