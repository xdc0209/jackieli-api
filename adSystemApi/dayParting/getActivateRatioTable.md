# 获取分时段数据-激活率对比## 描述
> 提供分时段数据-激活率对比

## URL
> [http:// 192.168.10.168:8081/ad/dayParting/getActivateRatioTable.do](http://dataviewer.ilongyuan.com.cn/ad/dayParting/getActivateRatioTable.do)

## 支持格式
> JSON

## HTTP请求方式
> POST

## 请求参数
> |参数|必选|类型|说明|
|:-----  |:-------|:-----|-----                               |
|appId  |true    |String|37b7ca345bf84d5a9515cfa023338c51  |
|platform    |true    |String   |1| 
|type    |true    |String   |1：往期对比推广活动；2：往期对比 推广活动组；3：活动对比 推广活动；4：活动对比 推广活动组| 
|promoteValue    |true    |String   |根据type类型传入相应的值|
|startDate    |true    |date   |2017-03-05 |
|endDate    |true    |date   |2017-03-05|   


## 返回字段（往期对比）
> |返回字段|示例|说明                              |
|:-----   |:----|:-----------------------------    |
| dh    |  |时间段|
|diffActivateRate|  |对比日激活率|
|selectActivateRate|  |查询日激活率|

## 返回字段（活动对比）
> |返回字段|示例|说明                              |
|:-----   |:----|:-----------------------------    |
| dh    |  |时间段|
|promoteKey1|  |选中对比活动/活动组id；其值为该表对应类型数值，此处为：激活率|
|promoteKey2|  |同上|
|...|  |同上|

