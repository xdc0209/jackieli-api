# 实时在线分析
> 在线分析模块中的acu/pcu分析

## URL
> http:// 192.168.10.70:8980/app/onlineAnalysis/getDailyOnlineUserAnalysisDataTable.do

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
|startDate|false|String|开始时间|
|endDate|false|String|结束时间|



## 返回字段
|返回字段|示例|说明                              |
|:-----   |:----|:-----------------------------    |
|dt      |    | 日期                    |
|acu     |  28 | acu                |
|pcu     |  100 | pcu                 |
|rate     |  0.28 | acu/pcu                 |

**19.实时累计数据**
# 实时累计数据

## URL
> http:// 192.168.10.70:8980/app/realTime/getRealTimeAccumulateDataTable.do

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
|---|----|----|----|
|onlineUserNum    | |实时在线人数|包含一个json对象key-value：<br>today:今天<br>lastDay:昨天 <br>last7Day:前7天  <br>last30Day:前30天|
|activateDeviceNum| |激活设备数|同上|
|addUserNum       | |新增用户|同上|
|netActiveUserNum | |净活跃用户|同上|
|activeUserNum    | |总活跃用户数|同上|
|payMoney         | |付费金额|同上|
|payCount         | |付费次数|同上|
|payUserNum       | |付费用户数|同上|
|onlineApex       | |同时在线峰值|同上|
|gamePlayCount    | |游戏次数|同上|
|gamePlayAvgTime  | |平均每次游戏时长|同上|


