# 获取某渠道下的推广活动详情

## URL
> [http:// 192.168.10.168:8081/ad/promoteDetail/getPromoteDataDetailByChannel.do](http://dataviewer.ilongyuan.com.cn/ad/promoteDetail/getPromoteDataDetailByChannel.do)

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
|type    |true    |String   |查看方式：1:汇总、2:按天显示|  
|adChannelId  |true    |String   |广告渠道ID|  
## 返回字段
> |返回字段|示例|说明                              |
|:-----   |:----|:-----------------------------    |
|name        |  | 活动名称|
|detail      | 不显示，用于封装a标签|   详情链接       |
|clickNum    | |   点击总数       |
|clickDistinctNum | |   排重点击       |
|clickDayDistinctNum | |  按天排重点击       |
|activateNum | |  激活设备数       |
|activateRate | | 激活率        |
|registerNum | |    注册设备数     |
|registerRate | |   注册率      |
|addDevicePayNum | |    新增付费设备数     |
|addDevicePayMoney | |   新增用户付费金额      |
|activeDevicePayNum | |  总付费设备数       |
|activeDevicePayMoney | |   总付费      |
|retention1Rate | |  一日留存率     |
|retention3Rate | |     三日留存率  |
|retention7Rate | |    七日留存率   |
| retention30Rate | |   三十日留存率    |
|ltv0Pay | |  ltv0     |
|ltv7Pay | |    ltv7   |
|ltv30Pay | |   ltv30    |




