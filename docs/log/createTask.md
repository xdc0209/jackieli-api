# 新增下载任务

## URL
> [http:// 192.168.10.168:8081/log/createTask.do](http://dataviewer.ilongyuan.com.cn/log/createTask.do)

## 支持格式
> JSON

## HTTP请求方式
> POST

## 请求参数
> |参数|必选|类型|说明|
|:-----  |:-------|:-----|-----                               |
|appId    |true    |String(32)|游戏Id                          |
|platform    |true    |String(32)   |平台 |
|taskName  |true    |String(32)|任务名称 |
|startDate    |true    |String(32)   |开始时间 |
|endDate    |true    |String(32)   |结束时间 |
|eventName    |true    |String(32)   |事件名称 |


## 返回字段
> |返回字段|示例|说明                              |
|:-----   |:----|:-----------------------------    |
|isSuccess      |  true  | 是否成功                 |

## 接口示例
> 地址：[http://test.dataviewer.ilongyuan.com.cn/log/getTask.do?page=0&pageSize=10&appId=289ee05803487e57&platform=1](http://dataviewer.ilongyuan.com.cn/app/onlineAnalysis/adjacentLoginInternalTable.do)
``` javascript
{
    "channelMap": {
        "longyuan5": "longyuan5",
        "jinritt": "jinritt",
        "uctt": "uctt"
       .......
    },
    "isSuccess": true,
    "code": 0
}
```

