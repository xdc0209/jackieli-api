# 总体趋势-活跃

## 描述
> 游戏概况-总体趋势-活跃

## URL
> [http://192.168.10.117:8080/app/gameBasic/activeTable.do](http://dataviewer.ilongyuan.com.cn/app/gameBasic/activeTable.do)

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
|AddActiveUserProportion |0.5 |   新用户占有      |
|addActiveUserNum |2132|净活跃用户（新用户） |
|expectAddActiveUserNum |31231 |净活跃用户（老用户） |
|dt |1499184000000 |时间  |
|expectAddActiveUserProportion |0.5 |老用户占有  |
|dailyActiveUserNum  |123213| 总活跃用户 |
## 接口示例
> 地址：[http://192.168.10.117:8080/app/gameBasic/activeTable.do](http://dataviewer.ilongyuan.com.cn/app/gameBasic/activeTable.do？appId=289ee05803487e57&platform=1)
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
            "AddActiveUserProportion":0.0016260162601626016,
            "addActiveUserNum":2,
            "dt:1499184000000",
            "expectAddActiveUserNum":1228,
            "expectAddActiveUserProportion":0.9983739837398374,
            "dailyActiveUserNum":1230
        }
    ]
}
```

