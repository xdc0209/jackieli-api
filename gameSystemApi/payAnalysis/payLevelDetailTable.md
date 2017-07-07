# 付费档位-付费档位分析-详细

## 描述
> 付费分析-付费档位-付费档位分析-详细

## URL
> [http://192.168.10.111:8080/app/payAnalysis/payLevelDetailTable.do](http://dataviewer.ilongyuan.com.cn/app/payAnalysis/payLevelDetailTable.do)

## 支持格式
> JSON

## HTTP请求方式
> POST

## 请求参数
> |参数|必选|类型|说明|
|:-----  |:-------|:-----|-----|
|appId    |true    |String|游戏id |   
|platform    |true    |String|平台 | 
| payMoney    |true    |Int|档位 |   




## 返回字段
> |返回字段|示例|说明                              |
|:-----   |:----|:-----------------------------    |
| avgNum      |  1  | 等级  |
| dt      |  1489680000000  | 付费金额  |
|payNum	     |  1  | 付费次数  |
| totalMoney	     |  1  | 付费次数  |
| userNum	     |  1  | 付费次数  |




## 接口示例
> 地址：[http://192.168.10.111:8080/app/payAnalysis/payLevelBasicTable.do](http://dataviewer.ilongyuan.com.cn/app/payAnalysis/payLevelBasicTable.do)
``` javascript
{
    "channelMap": {
        "longyuan5": "longyuan5",
        "jinritt": "jinritt",
        "uctt": "uctt"
    },
    "total": 130,
    "data": [
        {
            "avgNum": "1.30", 
            "userNum": 54237, 
            "payMoney": "6.00", 
            "payNum": 70466, 
            "totalMoney": "422796.00", 
            "detail": "<a href='javascript:;' data-value=6.0> 详细</a>"
        }
    ]
}
```
