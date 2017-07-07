# 付费数据-付费分析

## 描述
> 付费分析-付费数据-付费分析

## URL
> [http://192.168.10.117:8080/app/payAnalysis/payMoneyAnalysisTable.do](http://dataviewer.ilongyuan.com.cn/app/payAnalysis/payMoneyAnalysisTable.do)

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
|dayPayUser |0 |每日付费玩家  |
|monthPayUser |0 | 每月付费玩家    |
|payMoneyRange |2|付费金额区间|
|weekPayUser |0|每周付费玩家 |

## 接口示例
> 地址：[http://192.168.10.117:8080/app/payAnalysis/payMoneyAnalysisTable.do](http://dataviewer.ilongyuan.com.cn/app/payAnalysis/payMoneyAnalysisTable.do?appId=289ee05803487e57&platform=1)
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
            "dayPayUser":0,
            "monthPayUser":0,
            "payMoneyRange":"1",
            "weekPayUser":0
        }
    ]
}
```

