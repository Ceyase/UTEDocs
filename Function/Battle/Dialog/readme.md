# 03-Dialog系列函数
### //注释：[]内为必填,{}内为选填
### Battle_EndDialog()
- 结束战斗框内对话框后进入下一回合
- 返回值：成功返回true，失败返回false

### Battle_SetDialogAutoEnd([逻辑型true/false])
- 设置战斗框内对话框是否自动结束
- 返回值：永远返回true

### Battle_IsDialogAutoEnd()
- 返回值：返回战斗框内对话框是否自动结束

### Battle_SetDialog([TEXT],{CHOICE},{LINE2})
- TEXT为任意字符串
- CHOICE和LINE2为逻辑型(true/false)
- 在大多数情况下,CHOICE和LINE2并不用设定
- 设置战斗框内对话框的文本
- 返回值：返回TEXT
