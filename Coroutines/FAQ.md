# 常见问题解答

### 协程可以在哪些平台上运行？

理论上支持除了HTML5之外的一切。到目前为止，我只在Windows上进行了测试。整个扩展都是原生GML编写的，所以它应该可以开箱即用。您可能会在某个不经常测试的平台上遇到特殊的错误。如果你发现了他们，请[报告](https://github.com/JujuAdams/Coroutines/issues)给我们。

### 此代码库的许可证是什么？我可以将其用于商业项目吗？

该库在[MIT许可](https://github.com/JujuAdams/Coroutines/blob/master/LICENSE)下发布。这意味着您可以将其用于任何您想要的目的，包括商业项目。你可以把我的名字放在你的感谢列表（Juju Adams）并且说谢谢，这对我来说意义重大，但你没有义务这样做。

### 我认为您缺少一个有用的功能，我希望您实现它！

很好！请提出[Issues](https://github.com/JujuAdams/Coroutines/issues)。Issues使协程的使用更有趣。而且这可以让我在公共交通上感到无聊时思考一些事情。

### 我发现了一个错误，解决问题的最佳方法是什么？

请提出[Issues](https://github.com/JujuAdams/Coroutines/issues)。Juju 每天都会检查 GitHub，错误修复通常会在几天后发布。你也可以去[Discord服务器](https://discord.gg/8krYCqr)上找我，但这并不能替代一个很好的清晰的错误报告。

### 帮我！我收到有关异步事件的编译错误。
由于 GMS2.3.6 更改了一些与异步事件相关的常量名称，低于 v2.3.6 的 GameMaker 版本将不可以编译此库。您可以通过在 GM 的文档中找到旧名称并将其插入自己的项目来解决此问题。

### 协程是否适用于[GMLive](https://yellowafterlife.itch.io/gamemaker-live)？
我不知道。

### 说到GMLive，其作者还通过GMEdit实现了协程。这个库有什么不同？
Vadim早在GameMaker Studio 2.3将匿名函数引入GML之前就编写了他的协程实现。这是一个非常聪明的技术解决方案，可以解决旧版GM中许多缺失的功能。 幸运的是，GameMaker现在更加灵活，这个库主要利用了新功能来实现协程。

### 谁写的代码？
这个库是由[@jujuadams](https://twitter.com/jujuadams)经过长时间修补GameMaker而建立和维护的。Juju参与了很多[商业GameMaker游戏](http://www.jujuadams.com/)。

### 我可以给你捐款吗？
谢谢你想表达你的感激之情，这对我个人来说确实意义重大——但我很幸运的能从Gamedev中获得稳定的收入。如果你想支持我的工作，请在你的游戏里给我一个名字就够了。