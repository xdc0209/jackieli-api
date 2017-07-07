# 付费档位-礼包喜好分析

## 描述
> 付费分析-付费档位-礼包喜好分析

## URL
> [http://192.168.10.117:8080/app/payAnalysis/giftAnalysisBasicTable.do](http://dataviewer.ilongyuan.com.cn/app/payAnalysis/giftAnalysisBasicTable.do)

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
|avgNum |0 |时间  |
|currencyType |0 | 货币种类    |
|detail |2|详细|
|giftId |"rslg.moonton.diamond_50601"|礼包ID |
|giftMoney |"6.00"|礼包金额 |
|payNum |23805|购买次数 |
|totalMoney |"142830.00"|总金额 |
|userNum |22829|购买人数 |

## 接口示例
> 地址：[http://192.168.10.117:8080/app/payAnalysis/giftAnalysisBasicTable.do](http://dataviewer.ilongyuan.com.cn/app/payAnalysis/giftAnalysisBasicTable.do？appId=289ee05803487e57&platform=1)
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
            "avgNum":"1.04",
            "currencyType":"CNY",
            "detail":"<a href='javascript:;' data-value=rslg.moonton.diamond_50601-6.0-CNY> 详细</a>",
            "giftId":"rslg.moonton.diamond_50601",
            "giftMoney":"6.00",
            "payNum":23805,
            "totalMoney":"142830.00",
            "userNum":22829
        }
    ]
}
```

