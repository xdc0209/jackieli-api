# 相邻启动间隔分布

## URL
> [http:// 192.168.10.111:8080/app/onlineAnalysis/adjacentLoginInternalTable.do?](http://dataviewer.ilongyuan.com.cn/app/onlineAnalysis/adjacentLoginInternalTable.do)

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
|:-----   |:------|:-----------------------------   |
|metricName |0~60分钟 |    相邻启动间隔值        |
|userNum |1234 |该间隔的启动人数   |

## 接口示例
> 地址：[http://test.dataviewer.ilongyuan.com.cn/app/onlineAnalysis/adjacentLoginInternalTable.do?page=0&pageSize=10&appId=289ee05803487e57&platform=1&startDate=&endDate=](http://dataviewer.ilongyuan.com.cn/app/onlineAnalysis/adjacentLoginInternalTable.do)
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
            "metricName": 0~60分钟,
            "userNum": 123
        }
    ]
}
```


