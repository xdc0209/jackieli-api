# 实时趋势

## 描述
> 游戏概况-实时统计-实时趋势

## URL
> [http://192.168.10.70:8980/app/realTime/getRealTimeTrendDataTable.do](http://dataviewer.ilongyuan.com.cn/app/realTime/getRealTimeTrendDataTable.do)

## 支持格式
> JSON

## HTTP请求方式
> POST

## 请求参数
|参数|必选|类型|说明|
|-----  |-------|-----|-----|
|appId    |true    |String|应用唯一编号 | 
|platform|true|String|平台|
|channelField|false|String|渠道id|
|areaField|false|String|区服|
|versionField|false|String|版本|
|table|true|String|表:<br>实时在线-->online;<br>激活设备-->activate_device；<br>新增用户-->add_user；<br>付费金额-->pay_money|

## 返回字段
|返回字段|示例|说明                              |
|:-----   |:----|:-----------------------------    |
|dm|00:05|分钟间隔|
|todayValue      |  | 今天对应表的值（所有表字段相同）                |
|lastDayValue     |  | 昨天对应表的值（所有表字段相同）                |
|last7DayValue     | | 前7天对应表的值（所有表字段相同）                 |
|last30DayValue     |  | 前30天对应表的值（所有表字段相同）             |

## 接口示例
> 地址：[http://192.168.10.70:8980/app/realTime/getRealTimeTrendDataTable.do](http://dataviewer.ilongyuan.com.cn/app/realTime/getRealTimeTrendDataTable.do)
``` javascript
{
    "channelMap": {
        "longyuan5": "longyuan5",
        "jinritt": "jinritt",
        "uctt": "uctt"
    },
    "data": [
        {
            "lastDayValue": 0, 
            "last30DayValue": 0, 
            "last7DayValue": 0, 
            "dm": "00:00", 
            "todayValue": 0
        }, 
        {
         "lastDayValue": 0, 
            "last30DayValue": 0, 
            "last7DayValue": 0, 
            "dm": "00:05", 
            "todayValue": 0
        }
      ]
}
```