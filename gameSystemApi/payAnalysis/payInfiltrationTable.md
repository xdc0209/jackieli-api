# 付费转化-付费渗透

## 描述
> 付费分析-付费转化-付费渗透

## URL
> [http://192.168.10.111:8080/app/payAnalysis/payInfiltrationTable.do?](http://dataviewer.ilongyuan.com.cn/app/payAnalysis/payInfiltrationTable.do)

## 支持格式
> JSON

## HTTP请求方式
> POST

## 请求参数
> |参数|必选|类型|说明|
|:-----  |:-------|:-----|-----                               |
|appId    |true    |String(32)|游戏Id                          |
|platform    |true    |String(32)   |平台 |
|type    |true    |String(32)   |类型字段:1-国家，2-地区，3-渠道，以后还会有增加 |

## 返回字段
> |返回字段|示例|说明                              |
|:-----   |:------|:-----------------------------   |
|item |国家/地区/渠道 |                         |
|avgARPU |352.3 |日均ARPU              |
|avgARPPU |352.3 |日均ARPPU              |
|avgPayRatio |0.3 |日均付费率              |

## 接口示例
> 地址：[http://test.dataviewer.ilongyuan.com.cn/app/payAnalysis/payInfiltrationTable.do?page=0&pageSize=10&appId=289ee05803487e57&platform=1&type=3&&startDate=&endDate=](http://dataviewer.ilongyuan.com.cn/app/payAnalysis/payInfiltrationTable.do)
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
            "item": 中国,
            "avgARPU": 123.3,
            "avgARPPU": 352.3,
            "avgPayRatio": 0.3
        }
    ]
}
```
