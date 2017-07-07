# 报表分析-月报表数据明细

## 描述
> 报表分析-月报表数据明细

## URL
> [http://192.168.10.117:8080/app/report/getMonthReportData.do](http://dataviewer.ilongyuan.com.cn/app/report/getMonthReportData.do)

## 支持格式
> JSON

## HTTP请求方式
> POST

## 请求参数
> |参数|必选|类型|说明|
|:-----  |:-------|:-----|-----|
|appKey   |true    |String(32)|游戏Id |
|platform    |true    |String(32)   |平台 |
|reportType    |true    |String(32)   |报表类型 |
|startDate    |true    |Date |开始时间 |
|endDate    |true    |Date   |结束时间 |

## 返回字段
> |返回字段|示例|说明            |
|:-----   |:------|:--------    |
|activateDeviceNum |{2017-07-04: 0} |对应日期的激活设备数  |
|activeUserNum |{2017-07-04: 0}  | 活跃玩家   |
|acu | {2017-07-04: 0} | ACU   |
|addDeviceNum |{2017-07-04: 0}  | 新增设备数   |
|addUserNum |{2017-07-04: 0}  | 新增玩家数   |
|addUserRetention1Num |{2017-07-04: 0}  | 新增玩家次日留存   |
|addUserRetention3Num |{2017-07-04: 0}  | 新增玩家3日留存   |
|addUserRetention7Num |{2017-07-04: 0}  | 新增玩家7日留存   |
|avgPlayNum |{2017-07-04: 0}  | 平均日游戏次数  |
|avgPlayTime |{2017-07-04: 0} | 平均日游戏时长   |
|deviceRetention1Num |{2017-07-04: 0}  | 设备次日留存   |
|deviceRetention3Num |{2017-07-04: 0}  | 设备3日留存   |
|deviceRetention7Num |{2017-07-04: 0} | 设备7日留存   ||
|pcu |{2017-07-04: 0} | PCU   |
|playNum |{2017-07-04: 0}  | 游戏次数   |
|userRegisterRatio |{2017-07-04: 0}  | 玩家转化率   |
|reportMonthBaseDataMap |  | 月报表数据   |

## 接口示例
> 地址：[http:// 192.168.10.117:8080/app/report/getMonthReportData.do](http://dataviewer.ilongyuan.com.cn/app/report/getMonthReportData.do？appId=289ee05803487e57&platform=1&reportType=month)
``` javascript
{
    "channelMap": {
        "longyuan5": "longyuan5",
        "jinritt": "jinritt",
        "uctt": "uctt"
    },
    "total": 130,
    "code": 0,
    "data": {
       "totalIncome": {
            "2017-06-01--2017-06-30": "0.00"
        }, 
        "activateDeviceNum": {
            "2017-06-01--2017-06-30": 0
        }, 
        "addDeviceNum": {
            "2017-06-01--2017-06-30": 0
        }, 
        "payUserRatio": {
            "2017-06-01--2017-06-30": "0.00"
        }  
    },
    "reportMonthBaseDataMap":[
        {
            "activateDeviceNum": "月设备激活", 
        "addDeviceNum": "月新增设备", 
        "addUserNum": "月新增玩家", 
        "activeUserNum": "月活跃玩家", 
        "avgUserPlayTime": "月平均时长", 
        "avgPlayOneTime": "平均每次游戏时长（分）", 
        "avgPlayNum": "平均游戏次数", 
        "addUserRetention1Num": "月新增玩家次日留存（%）", 
        "lossUserNum": "月流失玩家数量", 
        "lossRatio": "月流失率", 
        "refluxUserNum": "月回流玩家数", 
        "totalIncome": "月总收入金额（￥）", 
        "payUserNum": "月充值玩家数量（去重）", 
        "payUserRatio": "月玩家付费率", 
        "arpu": "ARPU", 
        "arppu": "ARPPU"
        }
    ],
    "commonReportConfig":[
            {
                  "id": 2, 
        "userId": 2, 
        "appId": 6, 
        "platform": "1", 
        "reportType": "month", 
        "emailList": "lilidong@dragonest.com", 
        "postTime": "12,-1,26", 
        "channelList": "xx,longyuan5", 
        "metricCollection": "{\"basicData\":\"addDeviceNum,totalIncome,activateDeviceNum,payUserRatio\"}", 
        "isSubscribe": "1", 
        "gmtCreate": 1487576345000, 
        "gmtModify": 1491902439000
            }
    ]
}
```


