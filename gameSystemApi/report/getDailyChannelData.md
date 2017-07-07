# 报表分析-渠道数据

## 描述
> 报表分析-渠道数据

## URL
> [http://192.168.10.117:8080/app/report/getDailyChannelData.do](http://dataviewer.ilongyuan.com.cn/app/report/getDailyChannelData.do)

## 支持格式
> JSON

## HTTP请求方式
> POST

## 请求参数
> |参数|必选|类型|说明|
|:-----  |:-------|:-----|-----|
|appId    |true    |String(32)|游戏Id |
|platform    |true    |String(32)   |平台 |
|reportType    |true    |String(32)   |报表类型 |
|channelList    |true    |String(32)   |渠道列表 |
|startDate    |true    |Date(   |开始时间 |
|endDate    |true    |Date   |结束时间 |

## 返回字段
> |返回字段|示例|说明            |
|:-----   |:------|:--------    |
|activateDeviceNum |{2017-07-05: 0} |设备激活  |
|activeUserNum | {2017-07-05: 0}| 活跃玩家    |
|addArpu |{2017-07-05: 0} | 新增ARPU    |
|addUserNum |{2017-07-05: 0} | 新增玩家   |
|arppu |{2017-07-05: 0} | ARPPU值   |
|arpu |{2017-07-05: 0} | arpu值   |
|income |{2017-07-05: 0} | 收入金额   |
|payNum |{2017-07-05: 0} | 付费次数   |
|payUserNum |{2017-07-05: 0} | 付费人数   |

## 接口示例
> 地址：[http://192.168.10.117:8080/app/report/getDailyChannelData.do](http://dataviewer.ilongyuan.com.cn/app/report/getDailyChannelData.do？appId=289ee05803487e57&platform=1&userType=1)
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
            "ios_srzz":{
                "activateDeviceNum":{"2017-07-05": 0},
                "activeUserNum":{"2017-07-05": 0},
                "addArpu":{"2017-07-05": 0},
                "addUserNum":{"2017-07-05": 0},
                "arppu":{"2017-07-05": 0},
                "arpu":{"2017-07-05": 0},
                "income":{"2017-07-05": 0},
                "payNum":{"2017-07-05": 0}
            }
        }
    ]
    "reportDailyChannelDataMap":[
        {
            "activateDeviceNum":"设备激活",
            "activeUserNum":"活跃玩家",
            "addArpu":"新增ARPU值",
            "addUserNum":"新增玩家",
            "arppu":"ARPPU值",
            "arpu":"ARPU值",
            "income":"收入金额（￥）",
            "payNum":"付费次数",
            "payUserNum":"付费人数"
        }
    ]
}
```

