# 推广活动—活动详情页面

## URL
> [http:// 192.168.10.168:8081/ad/promoteDetail/toOnePromoteDetailView.do](http://dataviewer.ilongyuan.com.cn/ad/promoteDetail/toOnePromoteDetailView.do)

## 支持格式
> JSON

## HTTP请求方式
> POST

## 请求参数
> |参数|必选|类型|说明|
|:-----  |:-------|:-----|-----                               |
|appId    |true    |String|游戏Id     |
|platform    |true    |String  |平台 |
|startDate    |true    |date   |2017-03-05 |
|endDate    |true    |date   |2017-03-05|  
|promoteId  |true    |String   |广告推广活动id|  
## 返回字段
> |返回字段|示例|说明                              |
|:-----   |:----|:-----------------------------    |
|appId       |  | 应用id|
|appName      | |   应用名      |
|platform    | |   平台       |
|startDate | |   开始时间       |
|endDate | |  结束时间      |
|promoteId | |  推广活动id（用于请求数据、不显示）   |
|promoteName | 推广活动：uc体育频道活动2|  推广活动名（用于显示在该页面顶部）    |




