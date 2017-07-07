# 获取获取作弊总览## 描述
> 提供作弊详情页面作弊总览数据

## URL
> [http:// 192.168.10.168:8081/ad/cheat/getCheatDetailTable.do](http://dataviewer.ilongyuan.com.cn/ad/cheat/getCheatDetailTable.do)

## 支持格式
> JSON

## HTTP请求方式
> POST

## 请求参数
> |参数|必选|类型|说明|
|:-----  |:-------|:-----|-----                               |
|appId    |true    |String|游戏Id      |
|platform    |true    |String|平台      |
|startDate    |true    |date   |2017-03-05 |
|endDate    |true    |date   |2017-03-05|   


## 返回字段
> |返回字段|示例|说明                              |
|:-----   |:----|:-----------------------------    |
| promote    |  | 推广活动|
|promoteId|  | 推广活动Id|
|clickNum     |  | 点击总数|
|clickDistinctNum     |  | 排重点击|
|exceptionClickNum     |  | 异常点击数|
|exceptionClickRate     |  |异常点击率|
|activateDeviceNum     |  |激活设备数|
|exceptionActivateDeviceNum     |  |异常激活设备数|
|exceptionActivateRate     |  |异常激活率|


