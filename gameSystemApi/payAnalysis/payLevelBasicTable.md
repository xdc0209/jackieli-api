# 付费档位-付费档位分析；付费行为-付费等级

## 描述
> 付费分析-付费档位-付费档位分析

> 付费分析-付费行为-付费等级

## URL
> [http://192.168.10.111:8080/app/payAnalysis/payLevelBasicTable.do](http://dataviewer.ilongyuan.com.cn/app/payAnalysis/payLevelBasicTable.do)

## 支持格式
> JSON

## HTTP请求方式
> POST

## 请求参数
> |参数|必选|类型|说明|
|:-----  |:-------|:-----|-----|
|appId    |true    |String|游戏id |    
|platform    |true    |String|平台 |   




## 返回字段
> |返回字段|示例|说明                              |
|:-----   |:----|:-----------------------------    |
|Level      |  1  | 等级  |
|payMoney      |  23.5  | 付费金额  |
|payNum	     |  1  | 付费次数  |

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
            "payMoney": "283014.00", 
            "payNum": 6413, 
            "Level": 26
        }
    ]
}
```
