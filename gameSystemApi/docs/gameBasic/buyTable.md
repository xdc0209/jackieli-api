# 总体趋势-付费用户追踪

## 描述
> 游戏概况-总体趋势-付费用户追踪

## URL
> [http://192.168.10.117:8080/app/gameBasic/buyTable.do](http://dataviewer.ilongyuan.com.cn/app/gameBasic/buyTable.do)

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
|:-----   |:------|:--------    |
|addUserTotalMoney |68 |   新增付费金额      |
|averageRevenuePerPayingUser |146.8|日ARRPU |
|averageRevenuePerUser |0.5967479674796748 |日ARPU |
|dt |1499184000000 |时间  |
|payActiveUserNum |5 |付费人数  |
|payAddUserNum  |123213| 新增付费人数 |
|payUserRate  |0.0040650406504065045| 日付费率 |
|totalMoney  |123213| 付费金额 |
## 接口示例
> 地址：[http://192.168.10.117:8080/app/gameBasic/buyTable.do](http://dataviewer.ilongyuan.com.cn/app/gameBasic/buyTable.do？appId=289ee05803487e57&platform=1)
``` javascript
{
    "channelMap": {
        "longyuan5": "longyuan5",
        "jinritt": "jinritt",
        "uctt": "uctt"
    },
    "total": 130,
    "code": 0,
    "data": [
        {
            "addUserTotalMoney":68,
            "averageRevenuePerPayingUser":146.8,
            "averageRevenuePerUser":0.5967479674796748,
            "dt":1499184000000,
            "payActiveUserNum":5,
            "payAddUserNum":1,
            "payUserRate":0.0040650406504065045,
            "totalMoney":734
        }
    ]
}
```