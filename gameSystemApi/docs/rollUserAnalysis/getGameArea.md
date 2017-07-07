# 滚服玩家-获取区服(用户)

## 描述
> 用户分析-滚服玩家-获取区服(用户)

## URL
> [http://192.168.10.111:8080/app/rollUserAnalysis/getGameArea.do?](http://192.168.10.111:8080/app/rollUserAnalysis/getGameArea.do?)

## 支持格式
> JSON

## HTTP请求方式
> POST

## 请求参数
>|参数|必选|类型|说明|
|:------|:-----|:----|:-----|
|appId|true|String(32)|游戏Id|
|platform|true|String(32)|平台|
|channelField|false|String(32)|渠道|

## 返回字段
>|返回字段|说明|示例|
|:-----|:----|:----|
|areaField|区服|20|
   
## 接口示例
> 地址：[http://192.168.10.111:8080/app/rollUserAnalysis/getGameArea.do?appId=112489499a11995c&platform=ios&channelId=longyuan](http://192.168.10.111:8080/app/rollUserAnalysis/getGameArea.do?appId=112489499a11995c&platform=ios&channelId=longyuan)
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
		   "areaField":20
        }
    ]
}  
```


