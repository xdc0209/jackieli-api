# 总体趋势-banner数据

## 描述
> 游戏概况-总体趋势-banner数据

## URL
> [http://192.168.10.117:8080/app/gameBasic/basicTotalTable.do](http://dataviewer.ilongyuan.com.cn/app/gameBasic/basicTotalTable.do)

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
|averageDailyActiveUserNum |12 |   平均活跃人数      |
|totalAddUserNum |34|累计新增用户  |
|totalDeviceAddUserNum |34 |累计新增设备 |
|totalFirstPayUserNum |34 |累计付费人数  |
|totalTotalMoney |34 |累计付费金额  |

## 接口示例
> 地址：[http://192.168.10.117:8080/app/gameBasic/basicTotalTable.do](http://dataviewer.ilongyuan.com.cn/app/gameBasic/basicTotalTable.do？appId=289ee05803487e57&platform=1)
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
            "averageDailyActiveUserNum":15034,
            "totalAddUserNum":354760,
            "totalDeviceAddUserNum":312666,
            "totalFirstPayUserNum":24024,
            "totalTotalMoney":9144732
        }
    ]
}
```

