# 有效玩家

## 描述
> 用户分析-有效玩家

## URL
> [http://192.168.10.117:8080/app/userAnalysis/effectiveUser.do](http://dataviewer.ilongyuan.com.cn/app/userAnalysis/effectiveUser.do)

## 支持格式
> JSON

## HTTP请求方式
> POST

## 请求参数
> |参数|必选|类型|说明|
|:-----  |:-------|:-----|-----|
|appId    |true    |String(32)|游戏Id |
|platform    |true    |String(32)   |平台 |
|userType:1 |true     |Integer | 用户类型，1：新增玩家 ，2：活跃玩家|

## 返回字段
> |返回字段|示例|说明            |
|:-----   |:------|:--------    |
|dt |1499184000000 |时间  |
|apkVersion |'unknown' | 游戏版本    |
|appId |2 | 游戏ID    |
|channelId |2|渠道ID|
|demension |2|指标维度 |
|effectiveUser1 |2|日有效玩家 |
|effectiveUser7 |2|7日有效玩家 |
|effectiveUser30 |2|30日有效玩家 |
|gameArea |2|游戏区服 |
|gmtCreate |2|记录创建时间 |
|gmtModify |2|记录修改时间 |
|id |2|记录编号 |
|platform |2|品台 |
|userType |2|用户类型 |

## 接口示例
> 地址：[http:// 192.168.10.117:8080/app/userAnalysis/effectiveUser.do](http://dataviewer.ilongyuan.com.cn/app/userAnalysis/effectiveUser.do？appId=289ee05803487e57&platform=1&userType=1)
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
            "apkVersion":"unknown",
            "appId":"289ee05803487e57",
            "channelId":"N",
            "demension":0,
            "dt":1499097600000,
            "effectiveUser1":10,
            "effectiveUser7":0,
            "effectiveUser30":0,
            "gameArea":"unknown",
            "gmtCreate":1499242154708,
            "gmtModify":1499242154708,
            "id":0,
            "platform":"1",
            "userType":0
        }
    ]
}
```

