# 大R详情-大R详情

## URL
> [http:// 192.168.10.168:8081/app/whaleUser/getLargeRDetail.do](http://dataviewer.ilongyuan.com.cn/app/whaleUser/getLargeRDetail.do)

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
|createDate |2017-05-11|新增日期  |
|lastLoginDate |yyyy-MM-dd HH:mm:ss|最后一次登录时间 |
|lastPayDate |yyyy-MM-dd HH:mm:ss|最后一次充值时间 |
|level |12 |当前等级 |
|becomeLargeRDate |yyyy-MM-dd|成为大R日期 |
|becomeLargeRMoney |123.21|成为大R当日充值金额 |
|accumulateMoney |123.21 |累计充值金额 |


## 接口示例
> ## URL
> [http:// 192.168.10.168:8081/app/whaleUser/getLargeRDetail.do](http://dataviewer.ilongyuan.com.cn/app/whaleUser/getLargeRDetail.do)

``` javascript
{
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
            "createDate": 2017-05-11,
            "lastLoginDate": 2017-05-11 10:15:12,
            "lastPayDate": 2017-05-11 10:15:12,
            "level": 18,
            "becomeLargeRDate": 2017-05-11,
            "becomeLargeRMoney": 11.12,
            "accumulateMoney": 12.12
        }
    ]
}
}
