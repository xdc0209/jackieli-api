# 获取某活动的总和数据

## URL
> [http:// 192.168.10.168:8081/ad/promoteDetail/getOnePromoteDetailSum.do](http://dataviewer.ilongyuan.com.cn/ad/promoteDetail/getOnePromoteDetailSum.do)

## 支持格式
> JSON

## HTTP请求方式
> POST

## 请求参数
> |参数|必选|类型|说明|
|:-----  |:-------|:-----|-----                               |
|appId    |true    |String|游戏Id                          |
|platform    |true    |String   |平台 |
|startDate    |true    |date   |2017-03-05 |
|endDate    |true    |date   |2017-03-05|  
|promoteId  |true    |String   |广告推广活动id|  
## 返回字段
> |返回字段|示例|说明                              |
|:-----   |:----|:-----------------------------    |
|clickSumNum    | |   点击总数       |
|activateSumNum | | 激活数        |
|natureActivateSumNum | |    自然激活     |
|activateRate | |   激活率      |
|addSumNum | |    注册数    |
|addRate | |   注册率      |
|income | |  收入       |
|paySumNum | |  付费人数    |
|loginSumNum | |  登陆数     |





