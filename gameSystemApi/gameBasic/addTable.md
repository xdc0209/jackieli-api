# 总体趋势-激活注册

## 描述
> 游戏概况-总体趋势-激活注册

## URL
> [http://192.168.10.117:8080/app/gameBasic/addTable.do](http://dataviewer.ilongyuan.com.cn/app/gameBasic/addTable.do)

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
|addUserNum |12 |   新增账号      |
|deviceActiveAddUserNum |34|新增激活设备 |
|deviceAddUserNum |34 |新增注册设备 |
|dt |1499184000000 |时间  |
|playerConversionRate |0.5 |注册转化率  |

## 接口示例
> 地址：[http://192.168.10.117:8080/app/gameBasic/addTable.do](http://dataviewer.ilongyuan.com.cn/app/gameBasic/addTable.do？appId=289ee05803487e57&platform=1)
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
            "addUserNum":2,
            "deviceActiveAddUserNum":2,
            "deviceAddUserNum":1,
            "dt":1499184000000,
            "playerConversionRate":0.5
        }
    ]
}
```

