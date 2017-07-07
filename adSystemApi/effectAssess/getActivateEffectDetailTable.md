# 获取激活效果详情## 描述
> 提供效果评价页面激活效果数据

## URL
> [http:// 192.168.10.168:8081/ad/effectAssess/getActivateEffectDetailTable.do](http://dataviewer.ilongyuan.com.cn/ad/effectAssess/getActivateEffectDetailTable.do)

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
|promoteId|  | 推广活动Id|
|activateNum     |  | 激活数|
|clickOnDay0     |  |当日点击激活数|
|clickOnDay1     |  |前一日点击激活数|
|clickOnDay2     |  |前二日点击激活数|
|clickOnDay3     |  |前三日点击激活数|
|clickOnDay4     |  |前四日点击激活数|
|clickOnDay5     |  |前五日点击激活数|
|clickOnDay6     |  |前六日点击激活数|
|clickOnDay7     |  |前七日点击激活数|
|clickOnDay0Ltv     |  |当日点击激活对应的30日LTV|
|clickOnDay1Ltv     |  |前一日点击激活对应的的30日LTV|
|clickOnDay2Ltv     |  |前二日点击激活对应的的30日LTV|
|clickOnDay3Ltv     |  |前三日点击激活对应的的30日LTV|
|clickOnDay4Ltv     |  |前四日点击激活对应的的30日LTV|
|clickOnDay5Ltv     |  |前五日点击激活对应的的30日LTV|
|clickOnDay6Ltv     |  |前六日点击激活对应的的30日LTV|
|clickOnDay7Ltv     |  |前七日点击激活对应的的30日LTV|

