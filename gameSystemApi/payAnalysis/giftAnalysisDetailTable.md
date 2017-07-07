# 付费档位-礼包喜好分析-详细

## 描述
> 付费分析-付费档位-礼包喜好分析-详细

## URL
> [http://192.168.10.117:8080/app/payAnalysis/giftAnalysisDetailTable](http://dataviewer.ilongyuan.com.cn/app/payAnalysis/giftAnalysisDetailTable)

## 支持格式
> JSON

## HTTP请求方式
> POST

## 请求参数
> |参数|必选|类型|说明|
|:-----  |:-------|:-----|-----|
|appId    |true    |String(32)|游戏Id |
|platform    |true    |String(32)   |平台 |
| giftData    |true    |String(32)   |礼包数据 |
## 返回字段
> |返回字段|示例|说明            |
|:-----   |:------|:--------    |
|avgNum |0 |人均充值次数  |
| dt | 1490284800000 | 日期   |
| payNum |31|充值次数 |
| totalMoney |"2720.00"|充值总额|
| userNum |31|充值人数 |


## 接口示例
> 地址：[http://192.168.10.117:8080/app/payAnalysis/giftAnalysisDetailTable.do?giftData=rslg.moonton.diamond_50008-68.0-CNY](http://dataviewer.ilongyuan.com.cn/app/payAnalysis/giftAnalysisDetailTable.do?giftData=rslg.moonton.diamond_50008-68.0-CNY)
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
            "dt": 1490284800000, 
            "avgNum": "1.29", 
            "userNum": 31, 
            "payNum": 40, 
            "totalMoney": "2720.00"
        }
    ]
}
```

