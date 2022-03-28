## Complementary Shaders —— 魔改自BSL的"完美"光影

------

### | 简要介绍

​		Complementary Shaders是一个Java版的光影包，修改自Capt Tatsu的"[BSL Shaders](https://www.curseforge.com/linkout?remoteUrl=https%253a%252f%252fbitslablab.com%252fbslshaders%252f)"。该光影包的最终目的是在一切方面都表现得出色。性能、游戏性、漂亮的外观、兼容性......应有尽有。Complementary Shaders将会尝试在Optifine的渲染管线的限制下为你提供最稳定的游戏体验。它运行的效率极高，支持几乎每一种GPU和驱动，兼容那些被认为是不可能兼容光影的mod，修复了从未有光影包修复过的bug，不用过多的特效来打搅你......最重要的是，它看起来真的很不错~
​		本光影包支持自动生成法线贴图功能(需要在光影设置界面手动开启)，这意味着任何纹理都能根据颜色的不同有“凹凸不平的效果”，无需纹理包支持。
​		除了兼容Optifine以外，本光影包还兼容[Iris Shader光影加载器](https://www.mcbbs.net/thread-1161271-1-1.html)
​		本帖除提供光影汉化文档以外，还同时提供已调好的配置文件，详见文件列表。

### **|** 视频展示

@[bilibili](https://www.bilibili.com/video/av633010892)

### **|** 图片展示

![](https://attachment.mcbbs.net/data/myattachment/forum/202110/02/165527iesb87kl4qeqqqea.jpg)

![](https://attachment.mcbbs.net/data/myattachment/forum/202109/20/084813ad1pn1jmlxefpi1i.jpg)

![](https://attachment.mcbbs.net/data/myattachment/forum/202109/20/084813xtx2ypgkagkpj1rr.jpg)

![](https://attachment.mcbbs.net/data/myattachment/forum/202109/20/084813s9uurpdrvr944rgr.jpg)

![](https://attachment.mcbbs.net/data/myattachment/forum/202110/02/165525ixg2pvpfkp0mep8x.jpg)

![](https://attachment.mcbbs.net/data/myattachment/forum/202109/20/085421o98j59mw504fwjwg.png)



### **|** 相关链接 & 许可相关

#### 相关链接

- 原贴地址：https://www.curseforge.com/minecraft/customization/complementary-shaders
- 官方Discord：[https://discord.com/invite/A6faFYt](https://discord.com/invite/A6faFYt)
- 搬运文档相关Github仓库：https://github.com/Miracle0565/ComplementaryShaders

#### 许可相关

- 光影包授权：作者保留所有权利
- 搬运贴原创内容(汉化文档等)：[知识共享署名-非商业性使用-相同方式共享 4.0 国际许可协议](https://creativecommons.org/licenses/by-nc-sa/4.0/)
- [搬运授权](https://attachment.mcbbs.net/data/myattachment/forum/202109/20/084813np733a77mwc65jj7.png)

### **|** 常见问题解答(FAQ)

#### 如何安装光影？

目前提供光影功能的 Mod 有 OptiFine 和 Iris Shaders，前者支持 Forge 加载器（可以通过 OptiFabric Mod 兼容 Fabric）而后者支持 Fabric 加载器。OptiFine 几乎支持所有的 Minecraft 版本，而 Iris Shaders 作为新兴的光影 Mod，目前只支持 1.16.5 及更高版本。一般情况下，OptiFine 是使用光影的最佳选择。

虽然 Iris Shaders 支持的游戏版本较少，但其支持的 Sodium Mod 对图像性能的优化效果显著，甚至优于 OptiFine。如果你游玩的版本能够使用Iris shader，不妨先尝试 Iris Shaders。

本帖提供基于[PCL2启动器](https://www.mcbbs.net/thread-719579-1-1.html)的安装教程。

##### 安装Iris shader

Iris Shader是一个Fabric mod，这意味着你需要安装Fabric loader和Fabric API来使用它。

- [【第一步 安装Fabric loader及Fabric API】](https://m1.miaomc.cn/uploads/20220328_119e0146ffd10.png)

- 【第二步 下载对应游戏版本的[Iris Shader光影加载器](https://modrinth.com/mod/iris/versions) 和 [Sodium](https://modrinth.com/mod/sodium/versions)】

- [【第三步 安装Iris Shader光影加载器和Sodium】](https://m1.miaomc.cn/uploads/20220328_a4ca85689228e.png)

- [【第四步 安装并启用光影包】](https://m1.miaomc.cn/uploads/20220328_9fc60ffeb3c45.png)

##### 安装Optifine

- [【OptiFine安装教程】](https://m1.miaomc.cn/uploads/20220328_e477aa2b9d666.png)

#### 	Mod兼容性问题解答：

你可以查阅[已知的mod兼容问题修复方式](https://www.mcbbs.net/plugin.php?id=link_redirect&target=https%3A%2F%2Fjustpaste.it%2F60cgu)，下面是汉化版的介绍：

- 为了兼容许多mod，你需要在光影的设置页面打开"兼容模式"(Compatibility Mode)。
- 确保你使用了最新的Optifine，除非你在游玩1.16.5。 在1.16.5中，有的mod对G7的兼容性更好，有的对G8的兼容性更好
- 星辉魔法(Astral Sorcery) 1.12.2版本: 打开mod配置文件，将 "S:weakSkyRenders" 设为 "0".
- 星辉魔法(Astral Sorcery) 1.15.2版本: 打开mod配置文件，将 "weakSkyRenders" 设为 "[0]".
- 星辉魔法(Astral Sorcery) 1.16.5版本: 打开mod配置文件，将 "skyRenderingEnabled" 设为 "[]".
- 高级火箭(Advanced Rocketry) : 打开mod配置文件，将 "B:overworldSkyOverride" 设为 "false".
- 植物魔法(Botania): 打开mod配置文件，将 "B:fancySkybox.enable" 和 "B:shaders.enabled" 设为 "false".
- 电脑(Computer Craft Tweaked): 打开mod配置文件，将 "S:monitor_renderer" 设为 "gui.computercraft:config.peripheral.monitor_renderer.vbo".
- 热动力学(Thermal Dynamics): 安装此mod：https://www.curseforge.com/minecraft/mc-mods/unifine
- 午夜(The Midnight) 1.12.2版本: 打开mod配置文件，将 "B:rift_shaders" 设为 "false".
- 交错次元/黑暗沼泽(The Betweenlands): 打开mod配置文件，将 "B:use_shader" 设为 "false".
- 老鼠(Rats): 打开视频设置 -> 性能 -> 将"快速渲染"设为"关"
- CoFH核心(CoFH Core): 打开mod配置文件，将 "Render Area Block Breaking" 设为 "false".
- 雪！真实的魔法！(Snow! Real Magic!) : 确保你的mod版本为 1.16.3-2.2.2 或更高
- 更好的末地Forge版本(BetterEnd Forge Port): 更新你的mod至最新版本
- 如果你安装了 实体渲染机制优化(Entity Culling): 打开mod配置文件，将 "entityShadowsCullingLessAggressiveMode" 设为 "true".
- 魔法艺术3：巧工魔艺(Mana and Artifice): 打开mod配置文件，将 "hudMode" 设为 "1".
- Psi: 打开mod配置文件，将 "useShaders" 设为 "false".
- 更多实用设备(Extra Utilities): 打开mod配置文件，将 "I:"Deep Dark"" 设为 "10".
- Clientcommands 1.16.5及以下版本: 唯一的修复方法就是扬了这个光影或扬了这个mod
- Clientcommands 1.17.1及以上版本: 确保你从GitHub上下载了最新版的mod
- 天境：重生(The Aether Reborn) 1.16版本: 打开mod配置文件，将 "Disables Aether custom skybox" 设为 "true".

#### 	天空显示出现问题，怎么办？

​		打开 ESC暂停界面 -> 选项 ->视频设置 -> 细节 -> 将"天空"设为"开"。

#### 	有什么是被"光追的"(Ray traced)？

​		光轴和反射是经过光追处理的。

#### 	如果想要更好的性能，我应该怎么设置？

- 确保“视频设置 -> 最大帧率”设置为“无限制”。 （请不要将其设置为“垂直同步”！）
- 降低渲染距离。 即使是一些非常强大的 PC 也不能处理超过 16 个区块。
- 转到“视频设置 -> 光影”并确保“Render Quality（渲染精细度）”和“Shadow Quality（阴影精细度）”都设置为 1x 。
- 转到“视频设置 -> 性能”并设置如下：
  - 区域渲染：开
  - 快速渲染：开
  - 快速运算：开
  - 智能动态材质：开
  - 平滑 FPS： 关
- 转到“视频设置 -> 细节”并将“实体渲染距离”设置为“50%”。
- 确保在“视频设置-> 品质”中将“各向异性过滤”设置为“关”。

### **|** 本帖更新日志

2021.09.20 本帖发布

2021.09.27 修正介绍

2021.09.30 汉化文档更新至4.2.1，新增配置文件分享、汉化安装教程等

2021.10.02 图片改为使用幻灯片展示

2021.10.03 贴内译名标准化+修正介绍

2021.10.08 更新汉化文件至4.2.2版本

2021.10.14 新增推荐栏

2021.10.17 修正4.2.2版本汉化文件中的部分错误(by@隐居小树) ，移除了forgecdn直链

2021.10.21 开启协同编辑

2021.11.24 更新mod兼容性提示

2021.11.27 更新至4.3版本，合并部分汉化(by@隐居小树)、修改许可

2021.12.15 更新汉化(by@隐居小树)，添加github链接，协同编辑天天掉，再坏就反馈版见吧(

2022.01.08 更新 FAQ （译自 [Discord](https://www.mcbbs.net/plugin.php?id=link_redirect&target=https%3A%2F%2Fdiscord.com%2Fchannels%2F744189556768636941%2F744266952230305803%2F744270916170809425)）

2022.01.21 更新汉化文档（[pr#2](https://github.com/Miracle0565/ComplementaryShaders/pull/2)）

2022.03.14 更新汉化文档（[pr#4](https://github.com/Miracle0565/ComplementaryShaders/pull/4)）by@隐居小树

2022.03.28 搬运贴Markdown重写(论坛 V4 更新)

