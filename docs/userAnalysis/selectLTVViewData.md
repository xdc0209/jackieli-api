# 用户价值LTV

## URL
> [http:// 192.168.10.111:8080/app/userAnalysis /selectLTVViewData.do](http://dataviewer.ilongyuan.com.cn/app/userAnalysis/selectLTVViewData.do)

## 支持格式
> JSON

## HTTP请求方式
> POST

## 请求参数
> |参数|必选|类型|说明|
|:-----  |:-------|:-----|-----|
|appId    |true    |String(32)|游戏Id |
|platform    |true    |String(32)   |平台 |
|type    |true    |String(32)    |类型字段：1-新增用户LTV，2-新增设备LTV|

## 返回字段
> |返回字段|示例|说明            |
|:-----   |:------|:--------    |
|dt |2017-02-16 |   日期        |
|num |2342 |数量：如果type = 1,则表示当日新增用户数量，如果type=2,则表示新增设备数量  |
|totalMoney1 |0.233532 |ltv1 |
|totalMoney2 |0.233532 |ltv2   |
|totalMoney3 |0.233532 | ltv3 |
|totalMoney4 |0.233532 | ltv4 |
|totalMoney5 |0.233532 | ltv5 |
|totalMoney6 |0.233532 |ltv6 |
|totalMoney7 |0.233532 |ltv7 |
|totalMoney15 |0.233532 |ltv15 |
|totalMoney30 |0.233532 |ltv30 |
|totalMoney60 |0.233532 |ltv60|
|totalMoney90 |0.233532 |ltv90|
|totalMoney120 |0.233532 |ltv120|
|totalMoney180 |0.233532 |ltv180 |



