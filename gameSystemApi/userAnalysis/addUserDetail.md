# 新增玩家-地区/国家/账号类型

## 描述
> 用户分析-新增玩家-地区/国家/账号类型

## URL
> [http://192.168.10.111:8080/app/userAnalysis/addUserDetail.do?](http://dataviewer.ilongyuan.com.cn/app/userAnalysis/addUserDetail.do?)

## 支持格式
> JSON

## HTTP请求方式
> POST

## 请求参数
> |参数|必选|类型|说明|
|:-----  |:-------|:-----|-----|
|appId  |true   |String(32)   |游戏Id|
|platform   |true   |String(32) |平台 |
|userType   |true   |String     |1-地区，2-国家，3-账户类型|

## 返回字段
> |返回字段|示例|说明           |
|:-----   |:------|:--------    |
|metric   | |地区/国家/账户类型|
|num    |456   |新增人数    |
|percent  |0.56   |百分比     |
                                 
## 接口示例
>地址：[http://192.168.10.111:8080/app/userAnalysis/addUserDetail.do?appId=112489499a11995c&platform=1&userType=1](http://dataviewer.ilongyuan.com.cn/app/userAnalysis/addUserDetail.do?appId=112489499a11995c&platform=1&userType=1)
``` javascript
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
            "metric": 'China',
            "num":152,
            "percent":0.56
        }
    ]
}
```