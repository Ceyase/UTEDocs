# 打字机指令：增强文字和对话效果

> 文档由 Hatty 在 Sam & Ilias 的帮助下编写，翻译由 天机Ceyase 进行。

text="* 你好，世界！";

- & - 将文本分割到下一行。

	例如 text="* 你好，世界！* 你好，世界！* 你好，世界！"; 将输出：

		* 你好，世界！ * 你好，世界！ * 你好，世界！ (文字会超出屏幕范围)。

	例如 text="* 你好，世界！&* 你好，世界！&* 你好，世界！"; 将输出：

		* 你好，世界！
		* 你好，世界！
		* 你好，世界！

- {choice X} - 添加交互式选项，供玩家选择！

	例如：text="* 你好，世界！&& {choice 0}选项 1 {choice 1}选项 2{choice 'TMP'}{pause}";

	重要提示：{choice 'TMP'} 必须添加到文本末尾，选择系统才能工作。把它想象成汽车的发动机！

- {clear} - 清除文本框。

    与 {pause} 结合使用时，可在玩家按键时打印额外的对话！

	例如 text="* 你好，世界！{pause}{clear}* 你今天好吗？"；首先会打印 "* 你好，世界！"，然后玩家按下一个键，清空文本框并打印 "* 你今天好吗？"。

- {color \`颜色名称\`} - 将整个文本染成您选择的颜色，并略有渐变。

	例如 text="{color \`yellow\`}* Hello world!"; 将把 "* Hello world!"染成渐变的黄色！

	注意：color 和 color_text 不能与"或'一起使用，必须使用`！

- {color_text \`颜色名称\`} - 将整个文本染成您选择的颜色，但没有渐变。

	例如，text="{color_text \`yellow\`}* Hello world!"; 将把 "* Hello world!"变成纯黄色！

    > 重要提示：如果不使用 {color_text \`white\`}，大多数白色文本（尤其是对话）都会出现深蓝色阴影，这只有在三角符文中才会出现

	> 要获得纯正的传说之下白色文本（无阴影），请在所有常规文本中使用 {color_text \`white\`}！

- {effect X} - 为文字添加炫酷效果。

	X=-1，无效果

	X=0，晃动文字！

	X=1，波浪文字 (小幽灵风格)

- {face X} - 为文本添加一个面部精灵。

    X 是面孔精灵的面孔 ID，定义在 `Objects > Text > text_typer > User Event 5 - Group & Macro` 用户事件。

	详情看文档："为 NPC 添加面孔/对话精灵"

- {pause} - 暂停文字或对话，直到玩家按下某个键。

	> text="* Hello {pause} world!"; 只有在第一次与 NPC 互动时才会打印 "hello"，之后按任何键都会打印 "world!"！

	与 {clear} 不同，因为文本框不会被清除。

	如果使用了 {choice}，则必须暂停文本的播放，直到玩家做出选择！

- {sleep X} - 将文本输出暂停 X 帧。

    > text="* Hello {sleep 10} world!"; 将使 "world "的输出延迟 10 帧。

- {speed X} - 加快或减慢文本速度。

	> -10 -4 -3 -2 -1 0  1  2  3  4  10 <br>
	> <---------------|--------------->

	数字越大（正数），速度越慢

	例如，text="{speed 10}* Hello world!"; 键出速度会非常慢！

- {voice X} - 添加语音提示，在输入文本时播放。X 是语音文件的语音 ID，定义在

    `Objects>Text>text_typer>User Event 5 - Group & Macro` 用户事件。