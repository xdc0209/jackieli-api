# 流失统计-流失和回流数

## URL
> [http:// 192.168.10.111:8080/app/userAnalysis /selectLossStatisticsOriginalData.do](http://dataviewer.ilongyuan.com.cn/app/userAnalysis/selectLossStatisticsOriginalData.do)

## 支持格式
> JSON

## HTTP请求方式
> POST

## 请求参数
> |参数|必选|类型|说明|
|:-----  |:-------|:-----|-----|
|appId    |true    |String(32)|游戏Id |
|platform    |true    |String(32)   |平台 |
|type    |true    |String(32)   |类型字段：1-新增用户流失，2-活跃用户流失，3-付费用户流失，4-新增设备流失，5-活跃设备流失，6-付费设备流失，7-新增用户回流，8-活跃用户回流，9-付费用户回流，10-新增设备回流，11-活跃设备回流，12-付费设备回流|

## 返回字段
> |返回字段|示例|说明            |
|:-----   |:------|:--------    |
|dt |2017-02-16 |   日期        |
|num |300 |数量：如果type = 1,则表示当日新增用户数量，如果type=1,则表示活跃用户数量,以此类推  |
|num1Day |233 |次日流失/回流   |
|num3Day |233 |3日流失/回流   |
|num7Day |233 |7日流失/回流   |
|num15Day |233 |15次日流失/回流  |
|num30Day |233 |30日流失/回流   |


