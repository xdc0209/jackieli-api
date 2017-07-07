# 滚服玩家

## 描述
> 用户分析-滚服玩家-数据概况

## URL
>[http://192.168.10.111:8080/app/rollUserAnalysis/getRollUser.do?](http://192.168.10.111:8080/app/rollUserAnalysis/getRollUser.do?)

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
|DAU|开启过应用的用户| 125|
|addUser|新增人数| 122|
|addRollUser|新增人数中滚服人数 |45|
|rollUserAmount|总滚服人数| 56|
|rollUserActivateRate|活跃人数中滚服人数占比| 0.5623|
|rollPayUser|滚服付费人数| 12|
|dayPayUser|当日付费人数| 45|
|rollPayUserRate|滚服付费人数占比|0.5623 |
|rollUserPayMoney|滚服付费金额|1545 |
|dayPayMoney|当日总付费金额|125 |
|rollUserPayMoneyRate|滚服付费金额占比|0.5623 |
|rollArpu|滚服arpu| 12.5632|
|rollArppu|滚服arppu|85.1545 |
|onlineDuration|在线时长|1211215 |
|startupTimes|启动次数|125 |
|retentionNum1Day|1天留存|56 |
|retentionNum2Day|2天留存|56 |
|retentionNum3Day|3天留存|56 |
|retentionNum4Day|4天留存|56 |
|retentionNum5Day|5天留存|56 |
|retentionNum6Day|6天留存|56 |
|retentionNum7Day|7天留存|56 |
|retentionNum15Day|15天留存|56 |
|retentionNum30Day|30天留存|56 |
|retentionNum60Day|60天留存|56 |
|retentionNum90Day|90天留存|56 |
  
## 接口示例
>地址：[http://192.168.10.111:8080/app/rollUserAnalysis/getRollUser.do?appId=6dba18fd57e443889dc45f93fd106561&platform=ios&channelId=longyuan&gameArea=20&startDate=2017-05-20"&endDate=2017-05-21](http://192.168.10.111:8080/app/rollUserAnalysis/getRollUser.do?appId=112489499a11995c&platform=ios&channelId=longyuan&gameArea=20&startDate=2017-05-20"&endDate=2017-05-21)     
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
            "dt": 1489161600000,
			"channel_id": longyuan,
			"gameArea": 20,
            "DAU": 36,
			"addUser":45,
			"addRollUser":23,
            "rollUserAmount":56,
			"rollUserActivateRate":0.5623,
			"dayPayUser":23,
			"rollPayUser":15,
			"rollPayUserRate":0.5623,
			"rollUserPayMoney":546,
			"dayPayMoney":2875,
			"rollUserPayMoneyRate":0.5623,
			"rollArpu":153.6,
			"rollArppu":115.2,
			"onlineDuration":14515,
			"startupTimes":2,
			"retentionNum1Day": 0,
			"retentionNum2Day": 0,
			"retentionNum3Day": 0,
			"retentionNum4Day": 0,
			"retentionNum5Day": 0,
			"retentionNum6Day": 0,
			"retentionNum7Day": 0,
			"retentionNum15Day": 0,
            "retentionNum30Day": 0,
            "retentionNum60Day": 0,
            "retentionNum90Day": 0
        }
    ]
}
```
