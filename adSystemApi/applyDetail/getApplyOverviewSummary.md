# 获取应用详情概览总数

## URL
> [http:// 192.168.10.168:8081/ad/applyDetail/getApplyOverviewSummary.do](http://dataviewer.ilongyuan.com.cn/ad/applyDetail/getApplyOverviewSummary.do)

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
> |返回字段             |示例|说明                |
|:-----   |:----|:----------------------------- |
|  clickSumNum         |   | 点击总数     |
|  activateSumNum      |   | 激活数       |
|  natureActivateSumNum|   | 自然激活||  activateRate        |   | 激活率|
|  addSumNum           |   | 注册数     |
|  natureAddNum        |   | 自然注册数|
|  addRate             |   | 注册率|
|  income              |   | 收入|
|  natureIncome        |   | 自然付费收入|
|  paySumNum           |   | 付费人数|
|  naturePaySumNum     |   | 自然付费人数|
|  loginSumNum         |   | 登陆数|
|  natureLoginSumNum   |   | 自然登陆数|


