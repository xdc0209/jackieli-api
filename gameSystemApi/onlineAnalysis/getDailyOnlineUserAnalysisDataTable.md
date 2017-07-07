# 在线分析-每日在线用户

## 描述
> 在线分析-在线分析-每日在线用户；在线分析模块中的acu/pcu分析

## URL
> [http://192.168.10.70:8980/app/onlineAnalysis/getDailyOnlineUserAnalysisDataTable.do](http://dataviewer.ilongyuan.com.cn/app/onlineAnalysis/getDailyOnlineUserAnalysisDataTable.do)

## 支持格式
> JSON

## HTTP请求方式
> POST

## 请求参数
|参数|必选|类型|说明|
|-----  |-------|-----|-----|
|appId    |true    |String|应用唯一编号 | 
|platform|true|String|平台|
|channelField|false|String|渠道id|
|areaField|false|String|区服|
|versionField|false|String|版本|
|startDate|false|String|开始时间|
|endDate|false|String|结束时间|



## 返回字段
|返回字段|示例|说明                              |
|:-----   |:----|:-----------------------------    |
|dt      |    | 日期                    |
|acu     |  28 | acu                |
|pcu     |  100 | pcu                 |
|rate     |  0.28 | acu/pcu                 |

## 接口示例
> 地址： [http://192.168.10.70:8980/app/onlineAnalysis/getDailyOnlineUserAnalysisDataTable.do](http://dataviewer.ilongyuan.com.cn/app/onlineAnalysis/getDailyOnlineUserAnalysisDataTable.do)
``` javascript
{
	 "msg": "success", 
    "channelMap": {
        "longyuan5": "longyuan5",
        "jinritt": "jinritt",
        "uctt": "uctt"
    },
    "total": 0, 
    "code": 200, 
    "data": [
        {
            "dt":43661,
            "acu":28,
            "pcu":100,
            "rate":0.28
        }
    ]
}
```

