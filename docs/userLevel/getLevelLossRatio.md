# 等级流失率

## URL
> [http:// 192.168.10.168:8081/app/userLevel/getLevelLossRatio.do](http://dataviewer.ilongyuan.com.cn/app/userLevel/getLevelLossRatio.do)

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
|num7DayRatio |0.52|七日流失率   |
|num14DayRatio |0.53 |14日流失率 |
|num30DayRatio |0.3 |30日流失率  |
|onlineDuration |141121 |在线时长-以秒为单位的整数  |

## 接口示例
> 地址：[http:// 192.168.10.168:8081/app/userLevel/getLevelLossRatio.do](http://dataviewer.ilongyuan.com.cn/app/userLevel/getLevelLossRatio.do)
``` javascript
{
    "channelMap": {
        "longyuan5": "longyuan5",
        "jinritt": "jinritt",
        "uctt": "uctt"
       .......
    },
    "total": 130,
    "code": 0,
    "data": [
        {
            "level": 13,
            "num7DayRatio": 0.3,
            "num14DayRatio": 0.3,
            "num30DayRatio": 0.3，
            "onlineDuration": 154646
        }
    ]
}
```
