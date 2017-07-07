# 指标验证-验证配置


## 描述
> 指标验证-验证配置

## URL
> [http://192.168.10.117:8080/app/metricCheck/selectAppIsSelected.do](http://dataviewer.ilongyuan.com.cn/app/metricCheck/selectAppIsSelected.do)

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
|appId |"289ee05803487e57"|游戏ID  |
|appName |"巨龙之战" |游戏名称  |
|checkFlag |1 |'验证标示，0：表示不验证，1：表示验证,-1：表示邮箱发送信息，此时app_name是发送人信息和密码，app_id是地址', |
|gmtCreate |"1489852800000" |记录创建时间  |
|gmtModify |"1489852800000" |记录修改时间  |
|id | 1 |编号  |
|resultDetail | "<span class="lookDetail" data-pass="1">详情</span>....|详情  |

## 接口示例
> 地址：[http://192.168.10.117:8080/app/metricCheck/selectAppIsSelected.do](http://dataviewer.ilongyuan.com.cn/app/metricCheck/selectAppIsSelected.do?appId=289ee05803487e57&platform=1)
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
            "id" :121,
            "appId" :"289ee05803487e57",
            "appName":"巨龙之战",
            "checkFlag":1,
            "gmtCreate":1489852800000,
            "gmtModify":1489852800000
        }
    ]
}
```

