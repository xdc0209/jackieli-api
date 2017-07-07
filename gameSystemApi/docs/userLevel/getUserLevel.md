# 等级详情


## 描述
> 等级分析-等级详情

## URL
> [http://192.168.10.168:8081/app/userLevel/getUserLevel.do](http://dataviewer.ilongyuan.com.cn/app/userLevel/getUserLevel.do)

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
|level |12 |   等级             |
|ActiveNum |145|活跃玩家数   |
|ActiveRatio |0.53 |活跃玩家百分比 |
|playNum |145|游戏次数   |
|playRatio |0.53 |游戏次数百分比 |
|onlineDuration |1221|升级时长，单位是秒，传整数   |
|payNum |12 |付费次数 |
|payMoney |12.56 |付费金额 |


## 接口示例
> ## URL
> [http://192.168.10.168:8081/app/userLevel/getUserLevel.do](http://dataviewer.ilongyuan.com.cn/app/userLevel/getUserLevel.do)

``` javascript
{
    "channelMap": {
        "longyuan5": "longyuan5",
        "jinritt": "jinritt",
        "uctt": "uctt"
    },
    "total": 13,
    "code": 0,
    "data": [
        {
            "level": 13,
            "ActiveNum": 145,
            "ActiveRatio": 0.23,
            "playNum": 13,
            "playRatio": 0.52,
            "onlineDuration": 121313,
            "payNum": 15,
            "payMoney": 18.21
        }
    ]
}
```
