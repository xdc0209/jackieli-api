## 龙渊数据平台API

> 作者：龙渊数据统计平台游戏统计系统（作者：李立冬 龙渊数据平台web前端工程师）

## 什么是接口文档

在项目开发中，web项目的前后端分离开发，APP开发，需要由前后端工程师共同定义接口，编写接口文档，之后大家都根据这个接口文档进行开发，到项目结束前都要一直维护。

## 为什么要写接口文档
- 项目开发过程中前后端工程师有一个统一的文件进行沟通交流开发
- 项目维护中或者项目人员更迭，方便后期人员查看

## 接口规范是什么
- 首先接口分为四部分：方法、uri、请求参数、返回参数
  - 1、方法:新增(post) 修改(put) 删除(delete) 获取(get)
  - 2、uri：以/a开头，如果需要登录才能调用的接口(如新增、修改；前台的用户个人信息，资金信息等)后面需要加/u，即：/a/u；中间一般放表名或者能表达这个接口的单词；get方法，如果是后台通过搜索查询列表，那么以/search结尾，如果是前台的查询列表，以/list结尾；url参数就不说了。
  - 3、请求参数和返回参数，都分为5列：字段、说明、类型、备注、是否必填字段是类的属性；说明是中文释义；类型是属性类型，只有String、Number、Object、Array四种类型；备注是一些解释，或者可以写一下例子，比如负责json结构的情况，最好写上例子，好让前端能更好理解；是否必填是字段的是否必填。
  - 4、返回参数结构有几种情况：
     - 1、如果只返回接口调用成功还是失败（如新增、删除、修改等），则只有一个结构体：code和message两个参数；
     - 2、如果要返回某些参数，则有两个结构体：
     - code/mesage/data
     - data里写返回的参数,data是object类型




