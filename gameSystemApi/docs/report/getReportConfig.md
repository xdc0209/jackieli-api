# 报表分析-自定义报表设置

## 描述
> 报表分析-自定义报表设置


## URL
> [http://192.168.10.117:8080/app/report/getReportConfig.do](http://dataviewer.ilongyuan.com.cn/app/report/getReportConfig.do)

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
|msg |"未查找到条件的报表配置" |查找信息(如果没有查找到配置则返回)  |
|commonReportConfig |见示例 |报表配置  |

## 接口示例
> 地址：[http://192.168.10.117:8080/app/report/getReportConfig.do](http://dataviewer.ilongyuan.com.cn/app/report/getReportConfig.do？appId=289ee05803487e57&platform=1&reportType=daily)
``` javascript
{
    "channelMap": {
        "longyuan5": "longyuan5",
        "jinritt": "jinritt",
        "uctt": "uctt"
    },
    "commonReportConfig":{
        "appId":6,
        "channelList":"xx",
        "emailList":"",
        "gmtCreate":1490932877000,
        "gmtModify":1499316501000,
        "id":2,
        "isSubscribe":"1",
        "metricCollection":"{"basicData":"activateDeviceNum,addDeviceNum,addUserNum,userRegisterRatio,activeUserNum,acu,pcu,userPlayNum,avgPlayTime,avgPlayNum,deviceRetention1Num,deviceRetention3Num,deviceRetention7Num,addUserRetention1Num,addUserRetention3Num,addUserRetention7Num,activeUserRetention1Num,activeUserRetention3Num,activeUserRetention7Num","payData":"income,payAddUserNum,payUserNum,payRatio,addArpu,activeArpu,addArppu,activeArppu","accumulateData":"totalActivateDeviceNum,totalAddUserNum,totalPayUserNum,totalPayRation,totalIncome,totalArpu,totalArppu","channelData":"activateDeviceNum,addUserNum,activeUserNum,income,payNum,payUserNum,arpu,arppu,addArpu"}",
        "platform":"1",
        "postTime":"0,-1,-1",
        "reportType":"daily",
        "userId":2
    }
}
```

