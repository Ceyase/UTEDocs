# Anim_Destroy {docsify-ignore-all}

## 描述
用于摧毁缓动实例的函数

## 语法
```gml
Anim_Destroy(target ,var_name* ,skip*);
```

## 参数
| 参数 | 类型 | 描述 |
| :-- | :-- | :-- |
| target | Real(Object)/Real(Instance)/global | 目标实例/物体/全局变量 |
| var_name | String | 变量名称 |
| skip | Bool | 是否跳过缓动过程，直接到达目标值 |

## 返回值
Bool 摧毁结果。

true 为成功，false 为失败。

## 例子
```gml
Anim_Destroy(target, "x", true);
```

假如之前我们创建了一个缓动进程，内容是让target的x变量缓动。

那么这行代码会跳过缓动，直接让x变成目标值。