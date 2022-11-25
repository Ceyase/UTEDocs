# Encounter_Set {docsify-ignore-all}

## 描述
设置指定ID的Encounter数据。

## 语法
```gml
Encounter_Set(id, enemy_0, enemy_1, enemy_2, menu_dialog, bgm*, flee_enabled*, pause_bgm*, quick*, soul_x*, soul_y*);
```

## 参数
| 参数 | 类型 | 描述 |
| :-- | :-- | :-- |
| id | Real | 你想要去设置的Encounter ID |
| enemy_0 | Real(Object) | 0号怪物的物体 |
| enemy_1 | Real(Object) | 1号怪物的物体 |
| enemy_2 | Real(Object) | 2号怪物的物体 |
| menu_dialog | String | 遭遇时出现的文本 |
| bgm* | Real(Sound) | 在战斗开始时播放的背景音乐 |
| flee_enabled* | Boolean | 是否在mercy菜单中显示“* Free”按钮 |
| pause_bgm* | Boolean | 战斗开始时是否暂停之前的背景音乐 |
| quick* | Boolean | 是否更快的显示遭遇动画 |
| soul_x* | Real | 遭遇动画中灵魂最终移动到的x位置 |
| soul_y* | Real | 遭遇动画中灵魂最终移动到的y位置 |

## Returns
Boolean

## 例子
```gml
Encounter_Set(1,-1,battle_enemy_dummy,-1,"* Dummy blocked the way",bgm_battle,false,true,true,0,0);
```
设置 encounter id **1** 的 encounter 数据。

第一个和第三个敌人是不存在的，而第二个是 **battle_enemy_dummy**。

遭遇时出现的文本为 **Dummy blocked the way**。

背景音乐为 **bgm_battle_pre**。

"\* Flee" 按钮将 **不会显示**。

相遇动画是 **快速的过去**。

灵魂最终移动到的位置是 **左上角**。