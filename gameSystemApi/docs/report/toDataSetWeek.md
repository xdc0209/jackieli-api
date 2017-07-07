# 报表分析-周自定义报表分析页面路由

## 描述
> 报表分析-周自定义报表分析页面路由

## URL
> [http:// 192.168.10.117:8080/app/report/toDataSetWeek.do](http://dataviewer.ilongyuan.com.cn/app/report/toDataSetWeek.do)

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
|mailPostHourMap | |邮件日发送时间  |
|mailPostWeekMap | |邮件周发送时间  |
|reportWeekBaseDataMap | | 基本数据    |

## 接口示例
> 地址：[http:// 192.168.10.117:8080/app/report/toDataSetWeek.do](http://dataviewer.ilongyuan.com.cn/app/report/toDataSetWeek.do？appId=289ee05803487e57&platform=1&reportType=week)
``` javascript
{
    "channelMap": {
        "longyuan5": "longyuan5",
        "jinritt": "jinritt",
        "uctt": "uctt"
    },
    "total": 130,
    "code": 0,
   "reportWeekBaseDataMap":
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
     },
    "mailPostWeekMap":{
        "1":"星期一",
        "2":"星期二",
        "3":"星期三",
        "4":"星期四",
        "5":"星期五",
        "6":"星期六",
        "7":"星期天"
    },
    "mailPostHourMap":{
        "0":"0:00",
        "1":"1:00",
        "2":"2:00",
        "3":"3:00",
        "4":"4:00",
        "5":"5:00",
        "6":"6:00",
        "7":"7:00",
        "8":"8:00",
        "9":"9:00",
        "10":"10:00",
        "11":"11:00",
        "12":"12:00",
        "13":"13:00",
        "14":"14:00",
        "15":"15:00",
        "16":"16:00",
        "17":"17:00",
        "18":"18:00",
        "19":"19:00",
        "20":"20:00",
        "21":"21:00",
        "22":"22:00",
        "23":"23:00"
    }
}
```

