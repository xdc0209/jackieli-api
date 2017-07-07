# 新增玩家

## 描述
> 用户分析-新增玩家-新增玩家

## URL
> [http://192.168.10.117:8080/app/userAnalysis/selectAddUserTable.do](http://dataviewer.ilongyuan.com.cn/app/userAnalysis/selectAddUserTable.do)

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
> |返回字段|示例|说明 |
|:-----   |:------|:--------    |
|dt |1499184000000 |时间  |
|addUserNum |2 | 新增账户数  |
|deviceActiveAddUserNum |2|新增激活设备数 |
|deviceAddRatio |0.5|注册转化率 |
|deviceAddUserNum |2|新增注册设备数 |

## 接口示例
> 地址：[http://192.168.10.117:8080/app/userAnalysis/selectAddUserTable.do](http://dataviewer.ilongyuan.com.cn/app/userAnalysis/selectAddUserTable.do？appId=289ee05803487e57&platform=1)
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
            "deviceAddRatio":0.5,
            "deviceAddUserNum":1,
            "dt":1499184000000
        }
    ]
}
```
