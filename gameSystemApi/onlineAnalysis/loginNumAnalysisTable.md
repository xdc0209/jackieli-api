# 启动次数分析-每日

## 描述
> 在线分析-在线分析-启动次数分析-每日

## URL
> [http:// 192.168.10.111:8080/app/onlineAnalysis/loginNumAnalysisTable.do?](http://dataviewer.ilongyuan.com.cn/app/onlineAnalysis/loginNumAnalysisTable.do)

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
|dt   |2017-02-16    |日期  |
|totalLoginNum |1234 |当日总的启动次数   |

## 接口示例
> 地址：[http://test.dataviewer.ilongyuan.com.cn/app/onlineAnalysis/loginNumAnalysisTable.do?page=0&pageSize=10&appId=289ee05803487e57&platform=1&startDate=&endDate=](http://dataviewer.ilongyuan.com.cn/app/onlineAnalysis/loginNumAnalysisTable.do)
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
            "dt": 2017-04,
            "totalLoginNum": 12300
        }
    ]
}
```
