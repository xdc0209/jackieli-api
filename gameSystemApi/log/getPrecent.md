# 获取任务处理进度

##描述
> 日志导出-获取任务处理进度

## URL
> [http:// 192.168.10.168:8081/log/getPrecent.do](http://dataviewer.ilongyuan.com.cn/log/getPrecent.do)

## 支持格式
> JSON

## HTTP请求方式
> POST

## 请求参数
> |参数|必选|类型|说明|
|:-----  |:-------|:-----|-----|
|id    |true    |int|编号 |               


## 返回字段
> |返回字段|示例|说明                              |
|:-----   |:----|:-----------------------------    |
|id      |  51  | 编号                     |
|precent     |  100 | 进度                 |

## 接口示例
> 地址：[http:// 192.168.10.168:8081/log/getPrecent.do?id=1](http://dataviewer.ilongyuan.com.cn/log/getPrecent.do)
``` javascript
{
    "channelMap": {
        "longyuan5": "longyuan5",
        "jinritt": "jinritt",
        "uctt": "uctt"
    },
    "id": 13,
    "code": 0,
    "precent": 100
}
```
