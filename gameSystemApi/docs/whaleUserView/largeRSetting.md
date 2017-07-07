# 大R设置

## 描述
> 鲸鱼用户-大R设置


## URL
> [http://192.168.10.168:8081/app/whaleUser/addConfig.do](http://dataviewer.ilongyuan.com.cn/app/whaleUser/addConfig.do)

## 支持格式
> JSON

## HTTP请求方式
> POST

## 请求参数
> |参数|必选|类型|说明|
|:-----  |:-------|:-----|-----|
|appId    |true    |String|游戏id |    
|largeRDayMoney    |true    |double|当日充值大于该值可成为大R |   
|largeRAccumulateMoney    |true    |double|累计充值大于该值可称为大R |   
|payLevel    |true    |list| "payLevel": [{"min": 1,"max": 10},{"min": 11,"max": 20}] |   
|notLoginDay    |true    |int|大R预警-未登陆天数 |   
|notPayDay    |true    |int|大R预警-未支付天数 |     
|potentialRMinDayMoney    |true    |double|潜力大R-当日充值最小值 |    
|potentialRMaxDayMoney    |true    |double|潜力大R-当日充值最大值 |   
|potentialRMinAccumulateMoney    |true    |double|潜力大R-累计充值最小值 |   
|potentialRMaxAccumulateMoney    |true    |double|潜力大R-累计充值最大值 |   



## 返回字段
> |返回字段|示例|说明                              |
|:-----   |:----|:-----------------------------    |
|double      |  0  | 0-成功，1-失败，403-无权限   |


## 接口示例
> 地址：[http://192.168.10.168:8081/app/whaleUser/addConfig.do](http://dataviewer.ilongyuan.com.cn/log/getPrecent.do)
``` javascript
{
    "channelMap": {
        "longyuan5": "longyuan5",
        "jinritt": "jinritt",
        "uctt": "uctt"
    },
    "code": 0
}
```