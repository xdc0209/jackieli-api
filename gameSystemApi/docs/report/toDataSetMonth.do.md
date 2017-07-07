# 报表分析-月自定义报表分析页面路由

## 描述
> 报表分析-月自定义报表分析页面路由

## URL
> [http://192.168.10.117:8080/app/report/toDataSetMonth.do](http://dataviewer.ilongyuan.com.cn/app/report/toDataSetMonth.do)

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
|mailPostMonthMap | |邮件月发送时间  |
|reportMonthBaseDataMap | | 基本数据    |

## 接口示例
> 地址：[http:// 192.168.10.117:8080/app/report/toDataSetMonth.do](http://dataviewer.ilongyuan.com.cn/app/report/toDataSetMonth.do?appId=289ee05803487e57&platform=1&reportType=month)
``` javascript
{
    "channelMap": {
        "longyuan5": "longyuan5",
        "jinritt": "jinritt",
        "uctt": "uctt"
    },
    "total": 130,
    "code": 0,
   "reportMonthBaseDataMap":
     {
  "activateDeviceNum":"月设备激活",         "addDeviceNum":"月新增设备",         "addUserNum":"月新增玩家",         "activeUserNum":"月活跃玩家",         "avgUserPlayTime":"月平均时长",         "avgPlayOneTime":"平均每次游戏时长（分）",         "avgPlayNum":"平均游戏次数",         "addUserRetention1Num":"月新增玩家次日留存（%）",         "lossUserNum":"月流失玩家数量",         "lossRatio":"月流失率",         "refluxUserNum":"月回流玩家数",         "totalIncome":"月总收入金额（￥）",         "payUserNum":"月充值玩家数量（去重）",         "payUserRatio":"月玩家付费率",         "arpu":"ARPU",         "arppu":"ARPPU"
     },
    "mailPostMonthMap":{
        "0" :"每月月末",
        "1" :"1",
        "2" :"2",
        "3" :"3",
        "4" :"4",
        "5" :"5",
        "6" :"6",
        "7" :"7",
        "8" :"8",
        "9" :"9",
        "10" :"10",
        "11" :"11",
        "12" :"12",
        "13" :"13",
        "14" :"14",
        "15" :"15",
        "16" :"16",
        "17" :"17",
        "18" :"18",
        "19" :"19",
        "20" :"20",
        "21" :"21",
        "22" :"22",
        "23" :"23",
        "24" :"24",
        "25" :"25",
        "26" :"26",
        "27" :"27",
        "28" :"28",
        "29" :"29",
        "30" :"30"
    }
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

