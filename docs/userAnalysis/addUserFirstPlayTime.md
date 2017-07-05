# 新增玩家-首次游戏时长
## URL
>[http://192.168.10.117:8090/app/userAnalysis/addUserFirstPlayTime.do](http://192.168.10.117:8090/app/userAnalysis/addUserFirstPlayTime.do?)

## 支持格式
> JSON

## HTTP请求方式
> POST

## 请求参数
>|参数|必选|类型|说明|
|:-----  |:-------|:-----|-----|
|appId  |true|String(32)|游戏ID|
|platform   |true   |String（32） |平台|
 
## 返回字段
> |返回字段|示例|说明           |
|:-----   |:------|:--------    |
|metric   |1-2|指标名|
|num    |456   |人数    |
|percent  |0.56   |百分比     |


## 接口示例
>地址：[http://192.168.10.117:8090/app/userAnalysis/addUserFirstPlayTime.do](http://192.168.10.117:8090/app/userAnalysis/addUserFirstPlayTime.do?appId=112489499a11995c&platform=1)
``` javascript
{
    {
    "channelMap": {
        "longyuan5": "longyuan5",
        "jinritt": "jinritt",
        "uctt": "uctt"
       .......
    },
    "total": 130,
    "code": 0,
    "data": [
        {
            "metric": '1-2',
            "num":152,
            "percent":0.56
        }
    ]
}
}
