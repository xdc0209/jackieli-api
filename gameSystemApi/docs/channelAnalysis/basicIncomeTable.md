
# 渠道分析-渠道收入总览

##描述
> 渠道分析-渠道收入总览

## URL
> [http://192.168.10.117:8080/app/channelAnalysis/basicIncomeTable.do](http://dataviewer.ilongyuan.com.cn/app/channelAnalysis/basicIncomeTable.do)

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
|addPayUserNum |123 |新增付费玩家  |
|avgDailyARPPU |0 | 日均ARRPU    |
|avgDailyARPU |0 | 日均ARPU    |
|detail |"app/channelAnalysis/channelIncome.do?appId=289ee05803487e57&platform=1&channel=amoby" | 详细   |
|avgDailyPayFrequency |2 | 日均付费次数   |
|avgDailyPayRatio |2 | 日均付费率   |
|avgDailyPayUserNum |2 | 日均付费人数   |
|channel |2 | 渠道   |
|income |2 | 收入   |

## 接口示例
> 地址：[http://192.168.10.117:8080/app/channelAnalysis/basicIncomeTable.do](http://dataviewer.ilongyuan.com.cn/app/channelAnalysis/basicIncomeTable.do？appId=289ee05803487e57&platform=1&userType=1)
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
            "addPayUserNum":0,
            "avgDailyARPPU":0,
            "avgDailyARPU":0,
            "avgDailyPayFrequency":0,
            "avgDailyPayRatio":0,
            "avgDailyPayUserNum":0,
            "channel":"amoby",
            "detail":"app/channelAnalysis/channelIncome.do?appId=289ee05803487e57&platform=1&channel=amoby",
            "income":0
        }
    ]
}
```
