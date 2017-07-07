# 渠道分析-渠道数量总览

##描述
> 渠道分析-渠道数量总览

## URL
> [http://192.168.10.117:8080/app/channelAnalysis/basicAmountTable.do](http://dataviewer.ilongyuan.com.cn/app/channelAnalysis/basicAmountTable.do)

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
|addUserNum |1499184000000 |新增玩家  |
|channel |'unknown' | 渠道    |
|channelRatio |0.00000217956569973867 | 渠道比重    |
|detail |"app/channelAnalysis/channelAmount.do?appId=289ee05803487e57&platform=1&channel=amoby" | 详细   |
|deviceActiveAddUserNum |2 | 激活设备   |
|deviceAddUserNum |2 | 新增设备   |
|deviceRatio |2 | 玩家转化率   |

## 接口示例
> 地址：[http://192.168.10.117:8080/app/channelAnalysis/basicAmountTable.do](http://dataviewer.ilongyuan.com.cn/app/channelAnalysis/basicAmountTable.do？appId=289ee05803487e57&platform=1&userType=1)
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
            "addUserNum":1,
            "channel":"amoby",
            "channelRatio":0.00000217956569973867,
            "detail":"app/channelAnalysis/channelAmount.do?appId=289ee05803487e57&platform=1&channel=amoby",
            "deviceActiveAddUserNum":1,
            "deviceAddUserNum":1,
            "deviceRatio":1
        }
    ]
}
```


