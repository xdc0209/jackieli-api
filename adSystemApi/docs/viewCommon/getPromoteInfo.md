# 获取推广活动信息## 描述
> 获取指定应用、指定平台所有推广活动以及推广活动组

## URL
> [http:// 192.168.10.168:8081/ad/viewCommon/getPromoteInfo.do](http://dataviewer.ilongyuan.com.cn/ad/viewCommon/getPromoteInfo.do)

## 支持格式
> JSON

## HTTP请求方式
> POST

## 请求参数
> |参数|必选|类型|说明|
|:-----  |:-------|:-----|-----      |
| appId    | true |String|应用id|
|platform| true |String|平台|

## 返回字段【adPromotePlanGroupList】说明
> |返回字段|示例|说明                              |
|:-----   |:----|:-----------------------------    |
| id    | 26 |推广活动组id|
|name| 推广活动组6 |推广活动组名称|

## 返回字段【adPromotePlanList】说明
> |返回字段|示例|说明                              |
|:-----   |:----|:-----------------------------    |
| id    | 6 |推广活动id|
| key   | 下文出现的所有packageId、adChannel、promoteId均为该值别名 |推广活动唯一标识|
|name| 推广活动6 |推广活动名称|

