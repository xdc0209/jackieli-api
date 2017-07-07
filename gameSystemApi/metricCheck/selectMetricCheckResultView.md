# 指标验证-验证结果

## 描述
> 指标验证-验证结果

## URL
> [http://192.168.10.117:8080/app/metricCheck/selectMetricCheckResultView.do](http://dataviewer.ilongyuan.com.cn/app/metricCheck/selectMetricCheckResultView.do)

## 支持格式
> JSON

## HTTP请求方式
> POST

## 请求参数
> |参数|必选|类型|说明|
|:-----  |:-------|:-----|-----|
|appId    |true    |String(32)|游戏Id |
|platform    |true    |String(32)   |平台 |
|reportType    |true    |String(32)   |报表类型 |

## 返回字段
> |返回字段|示例|说明            |
|:-----   |:------|:--------    |
|appId |"289ee05803487e57"|游戏ID  |
|appName |"巨龙之战" |游戏名称  |
|checkResult |1 |检查结果  |
|checkResultToHtmlString |"<span class="pass">已通过</span>" |检查结果  |
|dt |"1489852800000" |查找信息  |
|gmtCreate |"1489852800000" |记录创建时间  |
|gmtModify |"1489852800000" |记录修改时间  |
|id | 1 |编号  |
|resultDetail | "<span class="lookDetail" data-pass="1">详情</span>....|详情  |

## 接口示例
> 地址：[http:// 192.168.10.117:8080/app/report/getReportConfig.do](http://dataviewer.ilongyuan.com.cn/app/report/getReportConfig.do?appId=289ee05803487e57&platform=1&reportType=1)
``` javascript
{
    "channelMap": {
        "longyuan5": "longyuan5",
        "jinritt": "jinritt",
        "uctt": "uctt"
    },
    "total";39,
    "data":[
        {
            "appId":"289ee05803487e57",
            "appName":"巨龙之战",
            "checkResult":1,
            "checkResultToHtmlString":"<span class="pass">已通过</span>",
            "dt":1489852800000,
            "gmtCreate":1489954732000,
            "gmtModify":1489954732000,
            "id":1101,
            "resultDetail":"<span class="lookDetail" data-pass="1">详情</span>
        }
    ]
}
```