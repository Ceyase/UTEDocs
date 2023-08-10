# 02-Bullet系列函数
### //注释：[]内为必填,{}内为选填
### Battle_CallBulletEventSoulCollision()
- 使用此函数可以触发目前灵魂的用户事件"Bullet Collision”
- 返回值：成功则无返回值,失败则返回false
- PS:感觉没卵用的一个命令

### Battle_IsBulletValid([BULLET])
- BULLET为Object索引
- 直翻：检测攻击是否有效
- 实际功能：检测BULLET的父对象是否是battle_bullet
- 返回值：如果是，返回true，如果不是，返回false
