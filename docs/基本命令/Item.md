### //注释：[]内为选填
### Item_Add(ITEM)
- ITEM为Object索引
- 在玩家的物品栏中添加一个物品
- 返回值-成功添加(玩家背包物品数<8)返回true,否则(玩家背包物品数>8)返回false.

### Item_CallEvent(ITEM,EVENT,[SLOT])
- ITEM为Object索引
- 触发ITEM的EVENT用户事件,同时将ITEM移动到玩家背包的第SLOT个位置(PS:SLOT默认为-1.也就是直接消失)
- 返回值-成功触发(ITEM是物品且背包里SLOT的位置是空位)返回true,否则返回false.(PS:当EVENT事件不存在时也会返回true)

### Item_Get(SLOT)
- SLOT为整数型
- 获取背包的第SLOT个位置是什么物品
- 返回值-成功获取(背包里SLOT的位置不是空位)时返回物品索引,否则返回-1

### Item_GetArmor()
- 获取一个特定物品的名称
- 返回值-成功获取(之前有设置过)时返回物品索引,否则返回-1

### Item_SetArmor(ITEM)
- ITEM为Object索引
- 设置一个特定物品名称
- 与Item_GetArmor对应
- 返回值-成功设置(ITEM是物品)时返回true,否则返回false

### Item_GetName(ITEM)
- ITEM为Object索引
- 获取ITEM的_name变量(PS:不是物品的名称，仅仅是一个变量，可以随时在ITEM的创建事件中赋值)
- 返回值-成功获取(ITEM是物品)时返回变量,否则返回""

### Item_GetNumber()
- 获取玩家背包的物品数量
- 返回值-返回数字

### Item_GetTextEat(NAME)
- NAME为字符串
- 获取一串文本
- 文本为:You ate the NAME
- 返回值-返回文本

### Item_GetTextEquip(NAME)
- NAME为字符串
- 获取一串文本
- 文本为:You equiped the NAME
- 返回值-返回文本

### Item_GetTextHeal(HEAL,[LINE])
- HEAL为字符串
- LINE为逻辑性(默认为true)
- 获取一串文本
- 当玩家血量大于或等于上限值时，文本为:Your HP was maxed out.
- 当玩家血量小于上限值时，文本为:The ITEM was thrown away.(ITEM为物品名称)
- 返回值-返回文本

### Item_GetWeapon()
- 获取一个特定物品的名称
- 返回值-返回物品索引

### Item_SetWeapon(ITEM)
- ITEM为Object索引
- 设置一个特定物品名称
- 与Item_GetWeapon对应
- 返回值-成功设置(ITEM是物品)时返回true,否则返回false

### Item_IsSlotValid(SLOT)
- SLOT为整数型
- 返回值:当SLOT>=0且<8时返回true,否则返回false.

### Item_IsValid(ITEM)
- ITEM为Object索引
- 检测ITEM是否为物品
- 返回值:当ITEM或ITEM的父对象为item时返回true，否则返回false.

### Item_Remove(SLOT)
- SLOT为整数型
- 删除玩家背包里的第SLOT个物品
- 返回值:成功删除返回true,否则返回false

### Item_Set(SLOT,ITEM)
- SLOT为整数型
- ITEM为Object索引
- 在玩家背包的第SLOT添加ITEM
- 返回值:成功添加返回true,否则返回false

### Item_Update()
- 更新目前的物品栏
- 返回值:无返回值
