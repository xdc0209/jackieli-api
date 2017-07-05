# 用户分析-设备详情

## URL
> [http:// 192.168.10.168:8081/app/userAnalysis/equipmentDetail.do](http://dataviewer.ilongyuan.com.cn/app/userAnalysis/equipmentDetail.do)

## 支持格式
> JSON

## HTTP请求方式
> POST

## 请求参数
> |参数|必选|类型|说明|
|:-----  |:-------|:-----|-----|
|appId    |true    |String(32)|游戏Id |
|platform    |true    |String(32)   |平台 |
|userType    |true    |String   |1-新增玩家-机型，2-新增玩家-联网方式，3-新增玩家-移动运营商，4-活跃玩家-机型，5-活跃玩家-联网方式，6-活跃玩家-移动运营商 7-付费玩家-机型，8-付费玩家-联网方式，9-付费玩家-移动运营商|

## 返回字段
> |返回字段|示例|说明            |
|:-----   |:------|:--------    |
|metric |oppo/4G/移动 |   机型/联网方式/移动运营商        |
|userNum |300 |玩家数量   |
|percent |0.12 |百分比   |


## 接口示例
> ## URL
> [http:// 192.168.10.168:8081/app/userAnalysis/equipmentDetail.do](http://dataviewer.ilongyuan.com.cn/app/userAnalysis/equipmentDetail.do)

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
            "metric": 'oppo',
            "userNum": 300,
            "percent": 0.12
        }
    ]
}

```
