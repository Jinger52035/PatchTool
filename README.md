PatchTool是一款由UE开发的多功能的小工具
如果您在看过文档之后仍然对此有疑问，可以观看教程。
https://www.bilibili.com/video/BV1Cs8AeEEfL/
此外，因为软件还在积极更新中，每个版本有出入可以查看对应的文档。

补丁创建：
PatchTool可以比较两个文件夹之间的插件，并且生成差异文件，这个差异文件即可作为文件夹级别上的补丁。
因为制作理念初期就是为了方便更新一些简单的Pak,这边在结合HotPatcher打出补丁Pak,同时这并不是一款热更新工具，只是文件夹比较，
所以你的产品有C++更新，仍然可以用此实现更新。你的UE游戏可以只将最新的补丁文件传递给你的测试人员等，即可实现更新。

本人的单机游戏采用了这种方式：https://docs.qq.com/sheet/DWUZLYUJtSUtGbnhK?tab=BB08J2

补丁更新功能：

选择[Release[Old]] 即是旧的游戏文件，如果选择正确会出现对应的版本号，如果制作者第一次没有加入版本号，那么最原始的第一个版本是没有版本号的，确定路径正确即可。
选择Patch[New-Old] 是补丁文件的地址，如果选择了正确的路径，那么版本号也会更新出来对应的版本。点击开始更新后,即可开始更新。
补丁文件需要按照顺序更新，(未来PatchTool会支持多补丁导入)
比如你下载的是0.0.1发行包版本，应用0.0.2-0.0.1补丁，即可将自己本地的游戏更新到0.0.2.
同样如果你得游戏已经是0.0.2，应用0.0.3-0.0.2即可将游戏更新到0.0.3

memreport(UE内存可视化分析)：
memreport在打包Development后使用是最好的，如果在Editor使用可能会受到编辑器加载内存的影响。


FAQ：

1.我只能用PatchTool更新UE游戏吗？

A:不是，PatchTool只是根据文件夹比较，目标不一定是UE制作的产物，只是作者本人懒得制作网络下载功能的产物，一些小游戏团队可以利用这个实现游戏更新。
除此之外，直接比较两个文件夹的差异也是可以的，并非只是为了UE打包的游戏。

2.PatchTool开源嘛？

PatchTool使用了蓝图和C++，Github的LFS使用付费，是一个臃肿的产品，所以不上传源码。但是PatchTool会不断积极更新。

3.PatchTool免费嘛？

PatchTool完全免费

4.PatchTool开源信息

请遵守相关规定

https://www.bilibili.com/video/BV1jKEoznEi9
