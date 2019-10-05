# 限制程序

`此程序设定目的限制一些固定剧情战斗伤害过高或过低`

物理限制:

|属性|地址|值含义|
|--|--|--|
|武将限制|f8210+武将番号|限制下位|
|-|f8310+武将番号|限制上位|
|战斗限制(只适用于敌人)|f8410+战斗番号|限制下位|
|-|f8490+战斗番号|限制上位|

- 上位是整数0-255 
- 下位是小数 数值/255就是小数部分

`限制程序原理`:所有伤害必须经过限制程序

- 这时候可以调整所有人的攻击力的发挥状况
- 原来基础是1 最高可上调到25600% 最低可调到0% 一般20%-70%限制伤害输出即可