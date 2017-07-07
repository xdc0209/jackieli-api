# 未登陆玩家

## 描述
> 等级分析-未登陆玩家

## URL
> [http://192.168.10.168:8081/app/userLevel/getLevelLossDetail.do](http://dataviewer.ilongyuan.com.cn/app/userLevel/getLevelLossDetail.do)

## 支持格式
> JSON

## HTTP请求方式
> POST

## 请求参数
> |参数|必选|类型|说明|
|:-----  |:-------|:-----|-----|
|appId    |true    |String(32)|游戏Id |
|platform    |true    |String(32)   |平台 |
|type    |true    |String(32)|玩家类型 1-新增，2-活跃，3-付费 |
|dayType    |true    |String(32)   |7-7日，14-14日，30-30日 |

## 返回字段
> |返回字段|示例|说明            |
|:-----   |:------|:--------    |
|level |12 |   等级             |
|num |145|玩家数   |
|ratio |0.53 |百分比 |


## 接口示例
> ## URL
> [http:// 192.168.10.168:8081/app/userLevel/getLevelLossDetail.do](http://dataviewer.ilongyuan.com.cn/app/userLevel/getLevelLossDetail.do)

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
            "level": 13,
            "num": 145,
            "ratio": 0.23
        }
    ]
}
```

