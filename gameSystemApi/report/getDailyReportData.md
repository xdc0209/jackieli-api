# 报表分析-日报表数据明细

## 描述
> 报表分析-日报表数据明细

## URL
> [http://192.168.10.117:8080/app/report/getDailyReportData.do](http://dataviewer.ilongyuan.com.cn/app/report/getDailyReportData.do)

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
|startDate    |true    |Date(   |开始时间 |
|endDate    |true    |Date   |结束时间 |

## 返回字段
> |返回字段|示例|说明            |
|:-----   |:------|:--------    |
|activateDeviceNum |{2017-07-04: 0} |对应日期的激活设备数  |
|activeArppu |{2017-07-04: 0}  | 活跃ARPPU    |
|activeArpu |{2017-07-04: 0}  | 活跃ARPU    |
|activeUserNum |{2017-07-04: 0}  | 活跃玩家   |
|activeUserRetention1Num |{2017-07-04: 0} | 活跃玩家次日留存   |
|activeUserRetention3Num |{2017-07-04: 0}  | 活跃玩家3日留存    |
|activeUserRetention7Num | {2017-07-04: 0} | 活跃玩家7日留存    |
|acu | {2017-07-04: 0} | ACU   |
|addArppu | {2017-07-04: 0} | 新增ARPPU   |
|addArpu |{2017-07-04: 0} |新增ARPU   |
|addDeviceNum |{2017-07-04: 0}  | 新增设备数   |
|addUserNum |{2017-07-04: 0}  | 新增玩家数   |
|addUserRetention1Num |{2017-07-04: 0}  | 新增玩家次日留存   |
|addUserRetention3Num |{2017-07-04: 0}  | 新增玩家3日留存   |
|addUserRetention7Num |{2017-07-04: 0}  | 新增玩家7日留存   |
|avgPlayNum |{2017-07-04: 0}  | 平均日游戏次数  |
|avgPlayTime |{2017-07-04: 0} | 平均日游戏时长   |
|deviceRetention1Num |{2017-07-04: 0}  | 设备次日留存   |
|deviceRetention3Num |{2017-07-04: 0}  | 设备3日留存   |
|deviceRetention7Num |{2017-07-04: 0} | 设备7日留存   |
|income |{2017-07-04: 0}  | 收入   |
|payAddUserNum |{2017-07-04: 0}  | 新增付费玩家数   |
|payRatio |{2017-07-04: 0}  | 日付费率   |
|payUserNum |{2017-07-04: 0}  | 付费玩家数   |
|pcu |{2017-07-04: 0} | PCU   |
|totalActivateDeviceNum |{2017-07-04: 0}  | 累计激活设备数   |
|totalAddUserNum |{2017-07-04: 0}  | 累计新增玩家数   |
|totalArppu |{2017-07-04: 0}  | 累计ARPPU   |
|totalArpu |{2017-07-04: 0} | 累计ARPU   |
|totalIncome |{2017-07-04: 0}  | 累计收入金额   |
|totalPayRation |{2017-07-04: 0}  | 总体付费率   |
|totalPayUserNum |{2017-07-04: 0}  | 累计付费玩家   |
|userPlayNum |{2017-07-04: 0}  | 游戏次数   |
|reportDailyAccumulateDataMap | | 日报表累计数据  |
|reportDailyBaseDataMap | | 日报表基本数据  |
|reportDailyPayDataMap | | 日报表付费数据  |
|commonReportConfig|    | 报表配置 |

## 接口示例
> 地址：[http://192.168.10.117:8080/app/report/getDailyReportData.do](http://dataviewer.ilongyuan.com.cn/app/report/getDailyReportData.do？appId=289ee05803487e57&platform=1&userType=1)
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
            "activateDeviceNum":{"2017-07-04": 0},
            "activeArppu":{"2017-07-04": 0},
            "activeArpu":{"2017-07-04": 0},
            "activeUserNum":{"2017-07-04": 0},
            "activeUserRetention1Num":{"2017-07-04": 0},
            "activeUserRetention3Num":{"2017-07-04": 0},
            "activeUserRetention7Num":{"2017-07-04": 0},
            "acu":{"2017-07-04": 0},
            "addArppu":{"2017-07-04": 0},
            "addArpu":{"2017-07-04": 0},
            "addDeviceNum":{"2017-07-04": 0},
            "addUserNum":{"2017-07-04": 0},
            "addUserRetention1Num":{"2017-07-04": 0},
            "addUserRetention3Num":{"2017-07-04": 0},
            "addUserRetention7Num":{"2017-07-04": 0},
            "avgPlayNum":{"2017-07-04": 0},
            "avgPlayTime":{"2017-07-04": 0},
            "deviceRetention1Num":{"2017-07-04": 0},
            "deviceRetention3Num":{"2017-07-04": 0},
            "deviceRetention7Num":{"2017-07-04": 0},
            "income":{"2017-07-04": 0},
            "payAddUserNum":{"2017-07-04": 0},
            "payRatio":{"2017-07-04": 0},
            "payUserNum":{"2017-07-04": 0},
            "pcu":{"2017-07-04": 0},
            "totalActivateDeviceNum":{"2017-07-04": 0},
            "totalAddUserNum":{"2017-07-04": 0},
            "totalArppu":{"2017-07-04": 0},
            "totalArpu":{"2017-07-04": 0},
            "totalIncome":{"2017-07-04": 0},
            "totalPayRation":{"2017-07-04": 0},
            "totalPayUserNum":{"2017-07-04": 0},
            "userPlayNum":{"2017-07-04": 0},
            "userRegisterRatio":{"2017-07-04": 0}
        }
    ]
    "reportDailyAccumulateDataMap":[
        {
            "totalActivateDeviceNum":"累计激活设备",
            "totalAddUserNum":"累计新增玩家",
            "totalArppu":"累计ARPPU",
            "totalArpu":"累计ARPU",
            "totalIncome":"累计收入金额（￥）",
            "totalPayRation":"总体付费率（%）",
            "totalPayUserNum":"累计付费玩家"
        }
    ]
    "reportDailyBaseDataMap"[
        {
            "activateDeviceNum":"激活设备",
            "activeUserNum":"活跃玩家",
            "activeUserRetention1Num":"活跃玩家次日留存",
            "activeUserRetention3Num":"活跃玩家3日留存",
            "activeUserRetention7Num":"活跃玩家7日留存",
            "acu":"ACU",
            "addDeviceNum":"新增设备",
            "addUserNum":"新增玩家",
            "addUserRetention1Num":"新增玩家次日留存",
            "addUserRetention3Num":"新增玩家3日留存",
            "addUserRetention7Num":"新增玩家7日留存",
            "avgPlayNum":"平均日游戏次数",
            "avgPlayTime":"平均日游戏时长（分）",
            "deviceRetention1Num":"设备次日留存",
            "deviceRetention3Num":"设备三日留存",
            "deviceRetention7Num":"设备7日留存",
            "pcu":"PCU",
            "userPlayNum":"游戏次数",
            "userRegisterRatio":"玩家转化率"
        }
    ]
    "reportDailyPayDataMap":[
        {
            "activeArppu":"活跃ARPPU",
            "activeArpu":"活跃ARPU",
            "addArppu":"新增ARPPU",
            "addArpu":"新增ARPU",
            "income":"收入（￥）",
            "payAddUserNum":"新增付费玩家数量",
            "payRatio":"日付费率（%）",
            "payUserNum":"付费玩家数量"
        }
    ]
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
            "reportType":"daily",
            "userId":2
        }
    ]
}
```


