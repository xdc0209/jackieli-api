# 大R详情-大R档位

## URL
> [http:// 192.168.10.168:8081/app/whaleUser/getLargeGear.do](http://dataviewer.ilongyuan.com.cn/app/whaleUser/getLargeGear.do)

## 支持格式
> JSON

## HTTP请求方式
> POST

## 请求参数
> |参数|必选|类型|说明|
|:-----  |:-------|:-----|-----|
|appId    |true    |String(32)|游戏Id |
|platform    |true    |String(32)   |平台 |


## 返回字段
> |返回字段|示例|说明            |
|:-----   |:------|:-------- |
|gear |2k-5k | 档位（累计充值）|
|num |300 | 人数   |



## 接口示例
> ## URL
> [http:// 192.168.10.168:8081/app/whaleUser/getLargeGear.do](http://dataviewer.ilongyuan.com.cn/app/whaleUser/getLargeGear.do)

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
            "gear": ,
            "accountId": 55532
        }
    ]
}
}
