# 月付费率

## 描述
> 付费分析-付费转化-月付费率

## URL
> [http://192.168.10.111:8080/app/payAnalysis/payRatioMonthTable.do?](http://dataviewer.ilongyuan.com.cn/app/payAnalysis/payRatioMonthTable.do)

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
|payUserNum |123 |月付费人数                         |
|payRatio |0.2335233 |月付费率                             |

## 接口示例
> 地址：[http://test.dataviewer.ilongyuan.com.cn/app/payAnalysis/payRatioMonthTable.do?page=0&pageSize=10&appId=289ee05803487e57&platform=1&startDate=&endDate=](http://dataviewer.ilongyuan.com.cn/app/payAnalysis/payRatioMonthTable.do)
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
            "dt": 2017-04,
            "payUserNum": 123,
            "payRatio": 0.37733
        }
    ]
}
```
