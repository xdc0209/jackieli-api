# 获取对账详情
## 描述
> 描述：提供对账系统页面登陆设备数据，按推广、按时间 查看为同一接口，type类型加以区分；查看方式为日期，点击“汇总”链接时，采用当前接口，且type=“按推广方式查看”&startDate=${dt}&endDate=’’&…

## URL
> [http:// 192.168.10.168:8081/ad/reconcileAccount/getReconcileAccountDetailTable.do](http://dataviewer.ilongyuan.com.cn/ad/reconcileAccount/getReconcileAccountDetailTable.do)

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
|adChannel     |  | 推广活动|
|promoteId | |   推广活动Id（不显示，用于按推广活动查询详情链接参数）     |
|dt     |  | 日期（也用于按照日期方式查询详情链接参数）|
|clickNum     |  | 点击总数|
|clickDistinctNum     |  | 排重点击|
|activateNum     |  | 激活设备数|
|activateRate     |  | 激活率|
|addNum     |  | 注册设备数|
|payMoney     |  |回收|



