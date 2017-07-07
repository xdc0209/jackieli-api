# 在线习惯-平均游戏时长和次数

## 描述
> 在线分析-在线习惯-平均游戏时长和次数

## URL
> [http://192.168.10.117:8080/app/onlineAnalysis/timeNumberDailyTable.do](http://dataviewer.ilongyuan.com.cn/app/onlineAnalysis/timeNumberDailyTable.do)

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
|averageNum |2 | 每玩家游戏次数    |
|averageTime |2 | 每玩家游戏时长    |
|channelId |2|渠道ID|
|dateString |2|渠道ID|
|demension |2|指标维度 |
|gameArea |2|游戏区服 |
|gmtCreate |2|记录创建时间 |
|gmtModify |2|记录修改时间 |
|id |2|记录编号 |
|platform |2|平台 |
| playTotalNum |2122|游戏总次数 |
| playTotalTime |2322|游戏总时长 |
| userTotalNum |1322|玩家数量|
|userType |2|用户类型 |


## 接口示例
> 地址：[http://192.168.10.117:8080/app/onlineAnalysis/timeNumberDailyTable.do](http://dataviewer.ilongyuan.com.cn/app/onlineAnalysis/timeNumberDailyTable.do？appId=289ee05803487e57&platform=1&userType=1)
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
            "apkVersion":"N",
            "appId":"289ee05803487e57",
            "averageNum":1.37,
            "averageTime":120,
            "channelId":"N",
            "dateString":null,
            "demension":0,
            "dt":1499184000000,
            "gameArea":"N",
            "gmtCreate":1499244593460,
            "gmtModify":1499244593460,
            "id":0,
            "platform":"1",
            "playTotalNum":1681,
            "playTotalTime":147598,
            "userTotalNum":1230,
            "userType":0
        }
    ]
}
```
