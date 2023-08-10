# 04-Enemy系列函数
### //注释：[]内为必填,{}内为选填
### Battle_CallEnemyEvent([EVENT],{ENEMY})
- EVENT为字符串
- ENEMY为整数型
- ENEMY为怪物的战斗编号,默认为-1
- 触发指定ENEMY的用户事件EVENT
- 返回值：成功返回true，失败返回false

### Battle_GetEnemy([ENEMY])
- ENEMY为怪物的Object索引
- 返回值：ENEMY的战斗编号

### Battle_SetEnemy([ENEMY],[SLOT])
- ENEMY为怪物的Object索引
- SLOT为整数型
- 设置怪物的战斗编号
- 返回值：成功返回true，失败返回false

### Battle_GetEnemyNumber()
- 只有在战斗中才能使用
- 返回值：当前场上怪物的数量

### Battle_IsEnemySlotValid([ENEMY])
- ENEMY为整数型
- 该函数就是没有卵用
- 返回值：当ENEMY>=0且<=2时输出true,否之返回false

### Battle_IsEnemyValid([ENEMY])
- ENEMY为Object索引
- 返回值：如果ENEMY是怪物返回true，不是则返回false

### Battle_RemoveEnemy([ENEMY])
- ENEMY为怪物的Object索引
- 重置怪物属性(包括名字等......)
- 返回值：成功返回true，失败返回false

# 04-Enemy-Action系列函数
### Battle_GetEnemyActionName([ENEMY],[ACTION])
- ENEMY为怪物的Object索引
- ACTION为整数型
- 返回第ACTION个行动的名称 PS:ACTION必须>=0且<=6
- 返回值：成功返回名称，失败无返回值

### Battle_SetEnemyActionName([ENEMY],[ACTION],[TEXT])
- ENEMY为怪物的Object索引
- ACTION为整数型
- TEXT为任意字符串
- 设置第ACTION个行动的名称为TEXT PS:ACTION必须>=0且<=6
- 返回值：成功返回true，失败返回false

### Battle_GetEnemyActionNumber([ENEMY])
- ENEMY为怪物的Object索引
- 获取怪物的行动数量
- 返回值：成功返回数量，失败返回0

### Battle_SetEnemyActionNumber([ENEMY],[NUM])
- ENEMY为怪物的Object索引
- NUM为整数型
- 设置怪物的行动数量
- 返回值：成功返回true，失败返回false

# 04-Enemy-Center Pos系列函数
### Battle_GetEnemyCenterPosX([ENEMY])
- ENEMY为怪物的Object索引
- 获取怪物的X坐标
- 返回值：成功返回坐标，失败返回0

### Battle_GetEnemyCenterPosY([ENEMY])
- ENEMY为怪物的Object索引
- 获取怪物的Y坐标
- 返回值：成功返回坐标，失败返回0

### Battle_SetEnemyCenterPos([ENEMY],[X],[Y])
- ENEMY为怪物的Object索引
- X为整数型
- Y为整数型
- 设置怪物的坐标
- 返回值：成功返回true，失败返回false

#Enemy信息函数
### Battle_GetEnemyDEF([ENEMY])
- ENEMY为怪物的Object索引
- 获取怪物的防御值(DEF)
- 返回值：成功返回整数，失败返回0

### Battle_SetEnemyDEF([ENEMY],[DEF])
- ENEMY为怪物的Object索引
- DEF为整数
- 更改怪物的防御值(DEF)
- 返回值：成功返回true，失败返回false

### Battle_GetEnemyName([ENEMY])
- ENEMY为怪物的Object索引
- 获取怪物的名字
- 返回值：成功返回字符串，失败返回无

### Battle_SetEnemyName([ENEMY],[NAME])
- ENEMY为怪物的Object索引
- NAME为字符串
- 更改怪物的名字
- 返回值：成功返回true，失败返回false
