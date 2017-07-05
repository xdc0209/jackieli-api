# 流失统计-流失率

## URL
> [http:// 192.168.10.111:8080/app/userAnalysis /selectLossStatisticsPercentData.do](http://dataviewer.ilongyuan.com.cn/app/userAnalysis/selectLossStatisticsPercentData.do)

## 支持格式
> JSON

## HTTP请求方式
> POST

## 请求参数
> |参数|必选|类型|说明|
|:-----  |:-------|:-----|-----|
|appId    |true    |String(32)|游戏Id |
|platform    |true    |String(32)   |平台 |
|type    |true    |String(32)   |类型字段：1-新增用户流失率，2-活跃用户流失率，3-付费用户流失率，4-新增设备流失率，5-活跃设备流失率，6-付费设备流失率|

## 返回字段
> |返回字段|示例|说明            |
|:-----   |:------|:--------    |
|dt |2017-02-16 |   日期        |
|num |300 |数量：如果type = 1,则表示当日新增用户数量，如果type=2,则表示活跃用户数量,以此类推  |
|num1Day |0.2335233 |次日流失率   |
|num3Day |0.2335233 |3日流失率  |
|num7Day |0.2335233 |7日流失率 |
|num15Day |0.2335233 |15日流失率  |
|num30Day |0.2335233 |30日流失率   |


