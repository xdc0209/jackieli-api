# 删除下载任务

##描述
> 日志导出-删除下载任务

## URL
> [http://192.168.10.168:8081/log/delete.do](http://dataviewer.ilongyuan.com.cn/log/delete.do)

## 支持格式
> JSON

## HTTP请求方式
> POST

## 请求参数
> |参数|必选|类型|说明|
|:-----  |:-------|:-----|-----                               |
|id    |true    |int|编号             |   


## 返回字段
> |返回字段|示例|说明                              |
|:-----   |:----|:-----------------------------    |
|isSuccess  |  true  | 是否成功                 |

## 接口示例
> 地址：[http://test.dataviewer.ilongyuan.com.cn/log/delete.do?id=1](http://dataviewer.ilongyuan.com.cn/log/delete.do)
``` javascript
{
    "channelMap": {
        "longyuan5": "longyuan5",
        "jinritt": "jinritt",
        "uctt": "uctt"
    },
    "code": 0,
    "isSuccess" :true
}
```

