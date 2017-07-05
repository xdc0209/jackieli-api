# 用户分析-滚服设备

## URL
>[http://192.168.10.111:8080/app/rollDevAnalysis/getRollDev.do?](http://192.168.10.111:8080/app/rollDevAnalysis/getRollDev.do?)

## 支持格式
> JSON

## HTTP请求方式
> POST

## 请求参数
>|参数|必选|类型|说明|
|:------|:-----|:----|:-----|
|appId|true|String(32)|游戏Id|
|platform|true|String(32)|平台|
|channelField|false|String(32)|渠道|
|areaField|false|String(32)|区服|
|startDate|false|String(32)|开始时间|
|endDate|false|String(32)|结束时间|

## 返回字段
>|返回字段|说明|示例|
|:-----|:----|:----|
|dt|日期|2017-05-21|
|channelField|渠道|longyuan |
|areaField|区服|20 |
|DAU|活跃设备| 125|
|addDev|新增设备| 122|
|addRollDev|新增设备中滚服设备 |45|
|rollDevAmount|总滚服设备| 56|
|rollDevActivateRate|活跃设备中滚服设备占比| 0.5623|
|rollPayDev|滚服付费设备| 12|
|dayPayDev|当日付费设备| 45|
|rollPayDevRate|滚服付费设备占比|0.5623 |
|rollDevPayMoney|滚服付费金额|1545 |
|dayPayMoney|当日总付费金额|125 |
|rollDevPayMoneyRate|滚服付费金额占比|0.5623 |
|rollArpu|滚服arpu| 12.5632|
|rollArppu|滚服arppu|85.1545 |
|onlineDuration|在线时长|1211215 |
|startupTimes|启动次数|125 |
|retentionNum30Day|30天留存|56 |
|retentionNum60Day|60天留存|56 |
|retentionNum90Day|90天留存|56 |
  
## 接口示例
>地址：[http://192.168.10.111:8080/app/rollDevAnalysis/getRollDev.do?appId=6dba18fd57e443889dc45f93fd106561&platform=ios&channelId=longyuan&gameArea=20&startDate=2017-05-20"&endDate=2017-05-21](http://192.168.10.111:8080/app/rollDevAnalysis/getRollDev.do?appId=6dba18fd57e443889dc45f93fd106561&platform=ios&channelId=longyuan&gameArea=20&startDate=2017-05-20"&endDate=2017-05-21)
``` javascript
    {
    "channelMap": {
        "longyuan5": "longyuan5",
        "jinritt": "jinritt",
        "uctt": "uctt"
       .......
    },
    "total": 130,
    "code": 0,
    "data": [
        {
            "dt": 1489161600000,
			"channel_id": longyuan,
			"gameArea": 20,
            "DAU": 36,
			"addDev":45,
			"addRollDev":23,
            "rollDevAmount":56,
			"rollDevActivateRate":0.5623,
			"dayPayDev":23,
			"rollPayDev":15,
			"rollPayDevRate":0.5623,
			"rollDevPayMoney":546,
			"dayPayMoney":2875,
			"rollDevPayMoneyRate":0.5623,
			"rollArpu":153.6,
			"rollArppu":115.2,
			"onlineDuration":14515,
			"startupTimes":2,
            "retentionNum30Day": 0,
            "retentionNum60Day": 0,
            "retentionNum90Day": 0
        }
      ...
    ]
    }
```
