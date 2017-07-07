# 总体趋势-留存趋势

## 描述
> 游戏概况-总体趋势-留存趋势

## URL
> [http://192.168.10.117:8080/app/gameBasic/retentionTable.do](http://dataviewer.ilongyuan.com.cn/app/gameBasic/retentionTable.do)

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
|num |6831 |   新增付费金额      |
|retentionNum1Day |0|1日留存率 |
|retentionNum2Day |0|2日留存率 |
|retentionNum3Day |0|3日留存率 |
|retentionNum4Day |0|4日留存率 |
|retentionNum5Day |0|5日留存率 |
|retentionNum6Day |0|6日留存率 |
|retentionNum7Day |0|7日留存率 |
|retentionNum13Day |0|13日留存率 |
|retentionNum14Day |0|14日留存率 |
|retentionNum15Day |0|15日留存率 |
|retentionNum29Day |0|29日留存率 |
|retentionNum30Day |0|30日留存率 |
## 接口示例
> 地址：[http://192.168.10.117:8080/app/gameBasic/retentionTable.do](http://dataviewer.ilongyuan.com.cn/app/gameBasic/retentionTable.do？appId=289ee05803487e57&platform=1)
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
            "dt":1499184000000,
            "num":1230,
            "retentionNum1Day":0,
            "retentionNum2Day":0,
            "retentionNum3Day":0,
            "retentionNum4Day":0,
            "retentionNum5Day":0,
            "retentionNum6Day":0,
            "retentionNum7Day":0,
            "retentionNum13Day":0,
            "retentionNum14Day":0,
            "retentionNum15Day":0,
            "retentionNum29Day":0,
            "retentionNum30Day":0
        }
    ]
}
```

