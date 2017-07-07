# 详情-查看指定日期所有活动数据## 描述
> 按照日期查询下的详情链接（详情a标签）

## URL
> [http:// 192.168.10.168:8081/ad/reconcileAccount/getReconcileAccountByDate.do](http://dataviewer.ilongyuan.com.cn/ad/reconcileAccount/getReconcileAccountByDate.do)

## 支持格式
> JSON

## HTTP请求方式
> POST

## 请求参数
> |参数|必选|类型|说明|
|:-----  |:-------|:-----|-----                               |
|appId    |true    |String|游戏Id                          |
|platform    |true    |String  |平台 |
|date    |true    |date   |2017-03-05 |
## 返回字段
> |返回字段|示例|说明                              |
|:-----   |:----|:-----------------------------    |
|adChannel   |  | 推广活动|
|clickNum     |  | 点击总数|
|clickDistinctNum     |  | 排重点击|
|activateNum     |  | 激活设备数|
|activateRate     |  | 激活率|
|addNum     |  | 注册设备数|
|payMoney     |  |回收|




