# 付费转化

## 描述
> 付费分析-付费转化-付费转化

## URL
> [http://192.168.10.111:8080/app/payAnalysis/payConversionTable.do?](http://dataviewer.ilongyuan.com.cn/app/payAnalysis/payConversionTable.do)

## 支持格式
> JSON

## HTTP请求方式
> POST

## 请求参数
> |参数|必选|类型|说明|
|:-----  |:-------|:-----|-----                               |
|appId    |true    |String(32)|游戏Id                          |
|platform    |true    |String(32)   |平台 |

## 返回字段
> |返回字段|示例|说明                              |
|:-----   |:------|:-----------------------------   |
|dt   |2017-02-16    |日期  |
|firstDayPayUserNum |123 |新增付费玩家          |
|allPayUserNum |132 |累计付费玩家
|allPayRatio |0.2335233 |总体付费率           |

## 接口示例
> 地址：[http://192.168.10.111:8080/app/payAnalysis/payConversionTable.do?](http://dataviewer.ilongyuan.com.cn/app/payAnalysis/payConversionTable.do)
``` javascript
{
    "channelMap": {
        "longyuan5": "longyuan5",
        "jinritt": "jinritt",
        "uctt": "uctt"
    },
    "total": 130,
     "msg": "success", 
    "code": 200,
    "data": [
        {
            "dt": 1497196800000, 
            "allPayUserNum": 24548, 
            "firstDayPayUserNum": 0, 
            "allPayRatio": 0.06750316919514818
        }
    ]
}
```
