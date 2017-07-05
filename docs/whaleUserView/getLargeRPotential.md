# 潜力大R-潜力大R

## URL
> [http:// 192.168.10.168:8081/app/whaleUser/getLargeRPotential.do](http://dataviewer.ilongyuan.com.cn/app/whaleUser/getLargeRPotential.do)

## 支持格式
> JSON

## HTTP请求方式
> POST

## 请求参数
> |参数|必选|类型|说明|
|:-----  |:-------|:-----|-----|
|appId    |true    |String(32)|游戏Id |
|platform    |true    |String(32)   |平台 |
|rankType    |true    |int   |1-正序，2-倒序|

## 返回字段
> |返回字段|示例|说明            |
|:-----   |:------|:--------    |
|rank |12 |   排名        |
|accountId |55532 |用户Id   |
|country |中国 |国家 |
|channelId |longyuan |渠道   |
|gameArea |1 |区服 |
|level |12 |当前等级 |
|becomePotentialRDate |yyyy-MM-dd|成为潜力大R日期 |
|becomePotentialRMoney |123.21|成为潜力大R当日充值金额 |
|accumulateMoney |123.21 |累计充值金额 |


## 接口示例
> ## URL
> [http:// 192.168.10.168:8081/app/whaleUser/getLargeRPotential.do](http://dataviewer.ilongyuan.com.cn/app/whaleUser/getLargeRPotential.do)

``` javascript
{
    "channelMap": {
        "longyuan5": "longyuan5",
        "jinritt": "jinritt",
        "uctt": "uctt"
       .......
    },
    "total": 13,
    "code": 0,
    "data": [
        {
            "rank": 13,
            "accountId": 55532,
            "country": '中国',
            "channelId": 'longyuan',
            "gameArea": '一区',
            "level": 18,
            "becomePotentialRDate": 2017-05-11,
            "becomePotentialRMoney": 11.12,
            "accumulateMoney": 12.12
        }
    ]
}


