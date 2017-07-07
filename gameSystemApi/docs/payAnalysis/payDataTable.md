# 付费数据

## 描述
> 付费分析-付费数据-付费数据


## URL
> [http://192.168.10.117:8080/app/payAnalysis/payDataTable.do](http://dataviewer.ilongyuan.com.cn/app/payAnalysis/payDataTable.do)

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
|dt |1499184000000 |时间  |
|addUserPayNum |2 | 新增付费人数    |
|addUserTotalMoney |2|新增玩家付费金额|
|firstPayTotalMoney |2|首次付费玩家付费 |
|firstPayUserNum |2|首次付费人数 |
|payActiveUserNum |2|活跃付费人数 |
|payAddUserNum |2|新增付费人数 |
|payNum |2|总付费人数|
|totalMoney |2|总付费金额 |

## 接口示例
> 地址：[http://192.168.10.117:8080/payAnalysis/payDataTable.do](http://dataviewer.ilongyuan.com.cn/payAnalysis/payDataTable.do?appId=289ee05803487e57&platform=1)
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
            "addUserPayNum":0,
            "addUserTotalMoney":0,
            "dt":1499184000000,
            "firstPayTotalMoney":68,
            "firstPayUserNum":1,
            "payActiveUserNum":5,
            "payAddUserNum":0,
            "payNum":5,
            "totalMoney":734
        }
    ]
}
```