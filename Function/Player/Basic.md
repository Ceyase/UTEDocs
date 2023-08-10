# 01-Board系列函数
### //注释：[]内为必填,{}内为选填
### Player_CalculateDamage([DAMAGE],{MIN},{MAX})
- DAMAGE为整数
- MIN和MAX虽然是选填，但是完全忽略，填了会报错
- 计算伤害
- DAMAGE是正常伤害值，经过计算伤害最大值，敌人防御值，玩家攻击值......之后得出一个准确伤害值
- 返回值-返回加工后的伤害值

### Player_GetPlot()
- 获取Plot
- 返回值-获取后的变量

### Player_SetPlot([Plot])
- Plot可以是任何文本/索引/变量
- 设置Plot,与Player_GetPlot对应
- 返回值-永远返回true

### Player_GetRoomName([ROOM])
- ROOM为房间索引
- 获取房间名称
- 没太搞懂.....
- 返回值-当ROOM为-1时，返回"--",否则返回""

### Player_GetTextTyperChoice()
- 获取文本类型选择
- 返回值-返回最近一次text_typer的_choice变量

### Player_Heal([HEAL])
- HEAL为整数型
- 回复玩家HEAL点血量
- 注:当HEAL为负数时，将会给玩家扣HEAL点血(反向治疗)
- 返回值-始终返回true

### Player_Hurt([DAMAGE])
- DAMAGE为整数型
- 扣除玩家DAMAGE点血量
- 注:当DAMAGE为负数时，将会给玩家回复DAMAGE点血(反向扣血)
- 返回值-始终返回true

### Player_IsInBattle()
- 检测是否在战斗中
- 返回值-如果在战斗中返回true，否则返回false

### Player_Load([])
