# 01-Board系列函数
### //注释：[]内为必填,{}内为选填
### Battle_GetBoardSurface()
  - 获取战斗框的Surface(表面)
  - 返回值-Surface索引

### Battle_IsBoardTransforming()
  - 该命令可以检测战斗框的框即坐标有没有变动
  - 该命令只有在使用Anim插件移动时生效
  - 返回值-如果战斗框的大小和xy坐标都没有变动则返回false,否则返回true
