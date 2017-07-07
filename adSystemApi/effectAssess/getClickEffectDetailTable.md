# 获取点击效果详情## 描述
> 提供效果评价页面点击效果详情

## URL
> [http:// 192.168.10.168:8081/ad/effectAssess/getClickEffectDetailTable.do](http://dataviewer.ilongyuan.com.cn/ad/effectAssess/getClickEffectDetailTable.do)

## 支持格式
> JSON

## HTTP请求方式
> POST

## 请求参数
> |参数|必选|类型|说明|
|:-----  |:-------|:-----|-----                               |
|appId    |true    |String|游戏Id      |
|platform    |true    |String|平台      |
|promoteId    |false    |String|点击某一推广活动时必须，否则为空    |
|startDate    |true    |date   |2017-03-05 |
|endDate    |true    |date   |2017-03-05|   


## 返回字段
> |返回字段|示例|说明                              |
|:-----   |:----|:-----------------------------    |
| promote/dt     |  | 推广活动/日期（查看具体某个活动）|
|promoteId|  | 推广活动Id(点击)|
|clickNum     |  | 点击总数|
|clickDistinctNum     |  | 排重点击|
|clickDayDistinctNum     |  | 按天排重点击|
|activateInDay0     |  |当日激活数|
|activateInDay1     |  |后一日激活数|
|activateInDay2     |  |后二日激活数|
|activateInDay3     |  |后三日激活数|
|activateInDay4     |  |后四日激活数|
|activateInDay5     |  |后五日激活数|
|activateInDay6     |  |后六日激活数|
|activateInDay7     |  |后七日激活数|
|activateInDay0Ltv     |  |当日激活的30日LTV|
|activateInDay1Ltv     |  |后一日激活的30日LTV|
|activateInDay2Ltv     |  |后二日激活的30日LTV|
|activateInDay3Ltv     |  |后三日激活的30日LTV|
|activateInDay4Ltv     |  |后四日激活的30日LTV|
|activateInDay5Ltv     |  |后五日激活的30日LTV|
|activateInDay6Ltv     |  |后六日激活的30日LTV|
|activateInDay7Ltv     |  |后七日激活的30日LTV|

