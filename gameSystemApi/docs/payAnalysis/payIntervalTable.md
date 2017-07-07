# 付费行为-付费间隔

## 描述
> 付费分析-付费行为-付费间隔

## URL
> [http://192.168.10.111:8080/app/payAnalysis/payIntervalTable.do](http://dataviewer.ilongyuan.com.cn/app/payAnalysis/payIntervalTable.do)

## 支持格式
> JSON

## HTTP请求方式
> POST

## 请求参数
> |参数|必选|类型|说明|
|:-----  |:-------|:-----|-----|
|appId    |true    |String(32)|游戏id |    
|platform    |true    |String(32)|平台 |   
|type    |true    |String(32)|取值分别为1,2,3; 1：首冲游戏时间分布,2：二冲到首冲时间分布,3：三冲到二冲时间分布 |   



## 返回字段
> |返回字段|示例|说明                              |
|:-----   |:----|:-----------------------------    |
|payInterval      |  1-2小时  | 时间间隔  |
|userNum      |  20  | 付费人数  |
|percent	     |  25%  | 百分比 |

## 接口示例
> 地址：[http://192.168.10.111:8080/app/payAnalysis/payIntervalTable.do?type=1](http://dataviewer.ilongyuan.com.cn/app/payAnalysis/payIntervalTable.do?type=1)
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
            "userNum": 965, 
            "payInterval": "<10分钟", 
            "percent": "12.78%"
        }
    ]
}
```
