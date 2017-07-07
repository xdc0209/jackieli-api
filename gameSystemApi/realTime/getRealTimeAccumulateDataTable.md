# 实时累计数据

## 描述
> 游戏概况-实时统计-实时累计数据

## URL
> [http://192.168.10.70:8980/app/realTime/getRealTimeAccumulateDataTable.do](http://dataviewer.ilongyuan.com.cn/app/realTime/getRealTimeAccumulateDataTable.do)

## 支持格式
> JSON

## HTTP请求方式
> POST

## 请求参数
|参数|必选|类型|说明|
|-----  |-------|-----|-----|
|appId    |true    |String|应用唯一编号 | 
|platform|true|String|平台|
|channelField|false|String|渠道id|
|areaField|false|String|区服|
|versionField|false|String|版本|



## 返回字段
|返回字段|示例|说明|
|---|----|----|
|onlineUserNum  |实时在线人数|包含一个json对象key-value：<br>today:今天<br>lastDay:昨天 <br>last7Day:前7天  <br>last30Day:前30天|
|activateDeviceNum| 激活设备数|同上|
|addUserNum       | 新增用户|同上|
|netActiveUserNum | 净活跃用户|同上|
|activeUserNum    | 总活跃用户数|同上|
|payMoney         | 付费金额|同上|
|payCount         | 付费次数|同上|
|payUserNum       | 付费用户数|同上|
|onlineApex       | 同时在线峰值|同上|
|gamePlayCount    | 游戏次数|同上|
|gamePlayAvgTime  | 平均每次游戏时长|同上|

## 接口示例
> 地址：[http://192.168.10.70:8980/app/realTime/getRealTimeAccumulateDataTable.do](http://dataviewer.ilongyuan.com.cn/app/realTime/getRealTimeAccumulateDataTable.do)
``` javascript
{
    "channelMap": {
        "longyuan5": "longyuan5",
        "jinritt": "jinritt",
        "uctt": "uctt"
    },
    "data": [
        {
            "activateDevNum": {
                "addNum": 0, 
                "today": 0, 
                "lastDay": 0, 
                "last30Day": 0, 
                "last7Day": 0
            }, 
            "addUserNum": {
                "addNum": 0, 
                "today": 0, 
                "lastDay": 0, 
                "last30Day": 0, 
                "last7Day": 0
            }, 
            "netActiveUserNum": {
                "addNum": 0, 
                "today": 0, 
                "lastDay": 0, 
                "last30Day": 0, 
                "last7Day": 0
            }, 
            "payUserNum": {
                "addNum": 0, 
                "today": 0, 
                "lastDay": 0, 
                "last30Day": 0, 
                "last7Day": 0
            }, 
            "payMoney": {
                "addNum": 0, 
                "today": 0, 
                "lastDay": 0, 
                "last30Day": 0, 
                "last7Day": 0
            }, 
            "playGameTime": {
                "addNum": 0, 
                "today": 0, 
                "lastDay": 0, 
                "last30Day": 0, 
                "last7Day": 0
            }, 
            "payTotalMoney": {
                "addNum": 0, 
                "today": 0, 
                "lastDay": 0, 
                "last30Day": 0, 
                "last7Day": 0
            }, 
            "activeUserNum": {
                "addNum": 0, 
                "today": 0, 
                "lastDay": 0, 
                "last30Day": 0, 
                "last7Day": 0
            }, 
            "onlineUserNum": {
                "addNum": 0, 
                "today": 0, 
                "lastDay": 0, 
                "last30Day": 0, 
                "last7Day": 0
            }, 
            "payCount": {
                "addNum": 0, 
                "today": 0, 
                "lastDay": 0, 
                "last30Day": 0, 
                "last7Day": 0
            }, 
            "playGameCount": {
                "addNum": 0, 
                "today": 0, 
                "lastDay": 0, 
                "last30Day": 0, 
                "last7Day": 0
            }
        }
    ]
}
```

