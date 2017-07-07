# 获取日志页面数据

##描述
> 日志导出-获取日志页面数据

## URL
> [http://192.168.10.168:8081/log/getTask.do](http://dataviewer.ilongyuan.com.cn/log/getTask.do)

## 支持格式
> JSON

## HTTP请求方式
> POST

## 请求参数
> |参数|必选|类型|说明|
|:-----  |:-------|:-----|-----                               |
|appId    |true    |String(32)|游戏Id                          |
|platform    |true    |String(32)   |平台 |

## 返回字段
> |返回字段|示例|说明                              |
|:-----   |:----|:-----------------------------    |
|id       |  56  | 序号                   |
|taskName |78_heartbeat |    任务名称             |
|eventType | 注册 |事件类型   |
|taskTime |2017-03-01至2017-04-21|导出时间|
|createTime |2017-03-01 |创建时间  |
|state |1 |0，1-导出中，2-下载  |
|downHref |.../78_heartbeat.xlsx |下载链接  |



## 接口示例
> 地址：[http://test.dataviewer.ilongyuan.com.cn/log/getTask.do?page=0&pageSize=10&appId=289ee05803487e57&platform=1](http://dataviewer.ilongyuan.com.cn/app/onlineAnalysis/adjacentLoginInternalTable.do)
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
            "id": 1,
            "taskName": "78_heartbeat",
            "eventType": "注册",
            "taskTime": "2017-03-01至2017-04-21",
            "createTime": "2017-03-01",
            "state": 1,
            "downHref": ".../78_heartbeat.xlsx"
        }
    ]
}
```

