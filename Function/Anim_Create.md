# Anim_Create {docsify-ignore-all}

## 描述
用于简化实例变量缓动的过程，旨在使用一个函数，即可完成复杂的缓动过程。

## 语法
```gml
Anim_Create(target ,var_name ,tween ,ease ,start ,change ,duration ,delay* ,arg_0* ,arg_1*);
```

## 参数
| 参数 | 类型 | 描述 |
| :-- | :-- | :-- |
| target | Real(Object)/Real(Instance)/global | 目标实例/物体/全局变量 |
| var_name | String | 变量名称 |
| tween | Enum | Tween效果，详见枚举常量部分 |
| ease | Enum | Ease效果，详见枚举常量部分 |
| start | Real | 起始值 |
| change | Real | 变更值 |
| duration | Real | 持续时间 |
| delay* | Real | 延迟时间 |
| arg_0* | Real | 附加参数 1 |
| arg_1* | Real | 附加参数 2 |

## 返回值
Real(Object) 缓动实例。

若有多个目标实例，则会返回Array。

## 例子
```gml
Anim_Create(target, "x", ANIM_TWEEN.QUAD, ANIM_EASE.OUT, 100, 200, 15, 30);
```
使target物体的所有实例的x变量，使用EaseOutQuart效果，在15帧内从100增大200，延迟30帧执行。

ANIM_TWEEN.QUAD和ANIM_EASE.OUT均为插件的自定义枚举常量，详见枚举常量部分。