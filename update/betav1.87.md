# NTS2R beta v1.87 2018-02-14

- 1.更新了2018年LOGO，版本号1.87
- 2.大将系统重制
    - 新大将系统说明：大将技能属于光环类，可以带动全队能力提升，不同的武将提升属性值和种类各不相同。大将光环分为四大类。攻，提升全队伤害加成。防，提升全队防御加成。命，提升全队的物理命中和计策成功率。避，提升全队闪避。
    - 大将系统只对本方队伍起作用，敌方大将没有加成。为提升游戏的趣味性，并不是名将的大将属性设置一定比杂鱼高，所以野将中藏有惊喜。
- 3.更改暗杀计为落雷计，效果为每回合结束后落雷攻击，10个回合结束，可被解策。
    - 更改大将系统设定的地址：
    - 1F510-1F60F对应255个武将的大将类型（80攻，40防，20命，10避，00无大将效果）
    - 1F610-1F70F对应255个武将加攻数据（只有类型设置为80，在此填入数据才有效）
    - 1F710-1F80F对应255个武将加防数据（只有类型设置为40，在此填入数据才有效）
    - 1F810-1F90F对应255个武将加命数据（只有类型设置为20，在此填入数据才有效）
    - 1F910-1FA0F对应255个武将加避数据（只有类型设置为10，在此填入数据才有效）
- 修复剧情战自动计策变落雷计的问题
- 调整一些大将光环的平衡
- 会心丹效果改为2倍会心
- 调整捕将所需金钱
- 武将做为合成材料用掉后不会在野外出现
- 修复偶尔出现的战斗中军师计策显示bug
- 调整中了嘲骂计不能使用恢复丹药和招魂丹
- 修复偶尔出现的落雷计花屏问题
