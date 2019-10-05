# 武将合成

(默认设置全部是OFF状态)

现阶段武将合成是仿造173代码，融入了渣技术的产物，和捕将一样，也是测试系统，非特殊要求请勿尝试。

不可合成条件如下：
- 1.选择同一个人物
- 2.合成的人物在编成所/7人队伍中存在
- 3.此人物不可作为合成素材或者合成对象
- 4.合成的人物等级不足
- 5.此人物的状态必须是80/98/90 斩杀的不可合成

合成的bug：
- 当合成成功时，地图上可能会随机消失一个人物（NPC），重新进入该地图即可解决

合成算法:
- 1.武将1的番号“与”代码AA做与运算得出数据1
- 2.武将2的番号“与”代码55做与运算得出数据2
- 3.数据1+数据2=新武将番号

举例子：
- 如果武将1番号是60
    - 60的二进制是01100000
    - AA的二进制是10101010
    - 运算的结果是00100000=20
- 如果武将2番号是6E
    - 6E的二进制是01101110
    - 55的二进制是01010101
    - 运算的结果是01000100=44
- 新武将番号:20+44=64

- “与”运算：
    - 把数据转换成2进制 对应位置对应上
    - 对应位置“见0出0,全1出1”
    - [百度百科与运算介绍](https://baike.baidu.com/item/%E4%B8%8E/13025631)
    - [Wikipedia 逻辑连词](https://en.wikipedia.org/wiki/Logical_conjunction)

|设定属性|填写地址|填写值|
|--|--|--|
|不可合成素材的设定地址|F9810-F988F|人物番号|
|不可合成对象的设定地址|F9890-F990F|人物番号|
|等级限制设定|F9910+武将番号|限制等级|

- 测试系统，只做过基本测试。