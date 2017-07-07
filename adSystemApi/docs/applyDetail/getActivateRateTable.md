# 获取激活率详情

## URL
> [http:// 192.168.10.168:8081/ad/applyDetail/getActivateRateTable.do](http://dataviewer.ilongyuan.com.cn/ad/applyDetail/getActivateRateTable.do)

## 支持格式
> JSON

## HTTP请求方式
> POST

## 请求参数
> |参数|必选|类型|说明|
|:-----  |:-------|:-----|-----                               |
|appId    |true    |String(32)|游戏Id                          |
|platform    |true    |String(32)   |平台 |
|startDate    |true    |date   |2017-03-05 |
|endDate    |true    |date   |2017-03-05|  
## 返回字段
> |返回字段|示例|说明                              |
|:-----   |:----|:-----------------------------    |
|adChannel/ dt      |  | 渠道或者日期，（查看方式不同）|
|activateRate | |   激活率       |




