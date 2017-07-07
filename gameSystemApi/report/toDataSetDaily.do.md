# 报表分析-日自定义报表分析页面路由

## 描述
> 报表分析-日自定义报表分析页面路由

## URL
> [http:// 192.168.10.117:8080/app/report/toDataSetDaily.do](http://dataviewer.ilongyuan.com.cn/app/report/toDataSetDaily.do)

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

## 返回字段
> |返回字段|示例|说明            |
|:-----   |:------|:--------    |
|mailPostHourMap |{2017-07-05: 0} |邮件发送时间  |
|reportDailyBaseDataMap | {2017-07-05: 0}| 基本数据    |
|reportDailyPayDataMap |{2017-07-05: 0} | 付费数据    |
|reportDailyAccumulateDataMap | | 累计数据   |
|reportDailyChannelDataMap | | 渠道数据指标   |
|channelMap | | 渠道列表   |

## 接口示例
> 地址：[http:// 192.168.10.117:8080/app/report/toDataSetDaily.do](http://dataviewer.ilongyuan.com.cn/app/report/toDataSetDaily.do？appId=289ee05803487e57&platform=1&reportType=daily)
``` javascript
{
    "channelMap": {
        "longyuan5": "longyuan5",
        "jinritt": "jinritt",
        "uctt": "uctt"
    },
    "total": 130,
    "code": 0,
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

