# 报表分析-周报表数据明细

## 描述
> 报表分析-周报表数据明细

## URL
> [http://192.168.10.117:8080/app/report/getWeekReportData.do](http://dataviewer.ilongyuan.com.cn/app/report/getWeekReportData.do)

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
|addUserRetention7Num |{2017-07-04: 0}  | 新增玩家7日留存|
|avgPlayNum |{2017-07-04: 0}  | 平均周游戏次数  |
|avgPlayTime |{2017-07-04: 0} | 平均周游戏时长   |
|deviceRetention1Num |{2017-07-04: 0}  | 设备次日留存   |
|deviceRetention3Num |{2017-07-04: 0}  | 设备3日留存   |
|deviceRetention7Num |{2017-07-04: 0} | 设备7日留存   |
|pcu |{2017-07-04: 0} | PCU   |
|playNum |{2017-07-04: 0}  | 游戏次数   |
|userRegisterRatio |{2017-07-04: 0}  | 玩家转化率   |
|reportWeekBaseDataMap |  | 周报表数据   |

## 接口示例
> 地址：[http:// 192.168.10.117:8080/app/report/getWeekReportData.do](http://dataviewer.ilongyuan.com.cn/app/report/getWeekReportData.do？appId=289ee05803487e57&platform=1&reportType=week)
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
            "activateDeviceNum":{
                                "2017-06-15--2017-06-18": 317, 
                                "2017-06-19--2017-06-25": 524, 
                                "2017-06-26--2017-07-02": 581
            },
            "activeUserNum":{
                "2017-06-15--2017-06-18": 0, 
                "2017-06-19--2017-06-25": 11882,
                "2017-06-26--2017-07-02": 11635
            },
            "acu":{
                "2017-06-15--2017-06-18": 0,
                "2017-06-19--2017-06-25": 0, 
                "2017-06-26--2017-07-02": 0
            }
            "addDeviceNum":{
                "2017-06-15--2017-06-18": 238,
                "2017-06-19--2017-06-25": 414,
                "2017-06-26--2017-07-02": 481
                },
            "addUserNum":{
                "2017-06-15--2017-06-18": 407,
                 "2017-06-19--2017-06-25": 599, 
                 "2017-06-26--2017-07-02": 686
                 },
            "addUserRetention1Num":{
                "2017-06-15--2017-06-18": 0,
                 "2017-06-19--2017-06-25": 0, 
                 "2017-06-26--2017-07-02": 0
                 },
            "addUserRetention3Num":{
                "2017-06-15--2017-06-18": 0, 
                "2017-06-19--2017-06-25": 0,
                 "2017-06-26--2017-07-02": 0
                 },
            "addUserRetention7Num":{
                "2017-06-15--2017-06-18": 0,
                 "2017-06-19--2017-06-25": 0, 
                 "2017-06-26--2017-07-02": 0
                 },
            "avgPlayNum":{"2017-06-15--2017-06-18": 0,
             "2017-06-19--2017-06-25": "16.27", "2017-06-26--2017-07-02": "15.62"
             },
            "avgPlayTime":{"2017-06-15--2017-06-18": 0, "2017-06-19--2017-06-25": "777.34", "2017-06-26--2017-07-02": "755.43"
            },
            "deviceRetention1Num":{"2017-06-15--2017-06-18": 0, "2017-06-19--2017-06-25": 0, "2017-06-26--2017-07-02": 0
            },
            "deviceRetention3Num":{"2017-06-15--2017-06-18": 0, "2017-06-19--2017-06-25": 0, "2017-06-26--2017-07-02": 0
            },
            "deviceRetention7Num":{"2017-06-15--2017-06-18": 0, "2017-06-19--2017-06-25": 0, "2017-06-26--2017-07-02": 0
            },
            "pcu":{"2017-06-15--2017-06-18": 0, "2017-06-19--2017-06-25": 0, "2017-06-26--2017-07-02": 0
            },
            "playNum":{"2017-06-15--2017-06-18": 0, "2017-06-19--2017-06-25": 193263, "2017-06-26--2017-07-02": 181763
            },
            "userRegisterRatio":{"2017-06-15--2017-06-18": "1.28", "2017-06-19--2017-06-25": "1.14", "2017-06-26--2017-07-02": "1.18"
            },
        }
    ],
    "reportWeekBaseDataMap":[
        {
            "activateDeviceNum":"周设备激活",
            "activeUserNum":"活跃玩家",
            "acu":"ACU",
            "addDeviceNum": "周新增设备",
            "addUserNum":"周新增玩家",
            "addUserRetention1Num":"新增玩家次日留存",
            "addUserRetention3Num":"新增玩家3日留存",
            "addUserRetention7Num":"新增玩家7日留存",
            "avgPlayNum":"平均周游戏次数",
            "avgPlayTime":"平均周游戏时长（分）",
            "deviceRetention1Num":"设备次日留存",
            "deviceRetention3Num":"设备3日留存",
            "deviceRetention7Num":"设备7日留存",
            "pcu":"PCU",
            "playNum":"游戏次数",
            "userRegisterRatio":"玩家转化率"
        }
    ],
    "commonReportConfig":[
            {
                "appId":6,
                "channelList":"ios_srzz,xx",
                "emailList":"",
                "gmtCreate":1490932877000,
                "gmtModify":1498548346000,
                "id":2,
                "isSubscribe":"1",
                "metricCollection":"{"basicData":"activateDeviceNum,addDeviceNum,addUserNum,userRegisterRatio,activeUserNum,acu,pcu,userPlayNum,avgPlayTime,avgPlayNum,deviceRetention1Num,deviceRetention3Num,deviceRetention7Num,addUserRetention1Num,addUserRetention3Num,addUserRetention7Num,activeUserRetention1Num,activeUserRetention3Num,activeUserRetention7Num","payData":"income,payAddUserNum,payUserNum,payRatio,addArpu,activeArpu,addArppu,activeArppu","accumulateData":"totalActivateDeviceNum,totalAddUserNum,totalPayUserNum,totalPayRation,totalIncome,totalArpu,totalArppu","channelData":"activateDeviceNum,addUserNum,activeUserNum,income,payNum,payUserNum,arpu,arppu,addArpu"}",
                "platform":"1",
                "postTime":"0,-1,-1",
                "reportType":"week",
                "userId":2
            }
    ]
}
```


