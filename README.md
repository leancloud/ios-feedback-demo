## 介绍
这个是一个演示反馈功能用法的示例项目。

## 如何运行

1. 用XCode打开FeedbackDemo.xcodeproj，选择运行的scheme和设备，点击运行按钮或菜单`Product`->`Run`或快捷键`Command(⌘)`+`r`就可以运行此示例

2. 如果你想获取最新发布的SDK，你也可以使用`cocoapods`,将`Frameworks`目录下的文件删除，然后在终端执行代码:

	    pod install

    不出问题的话 1分钟即可完成所有设置, 并生成名为`FeedbackDemo.xcworkspace`的Xcode工作空间，用Xcode打开它，按第1种介绍的方法运行即可

----

## 使用说明

### 替换 App 信息

示例使用的是公共的 app id 和 app key，您可以在`AppDelegate.m`修改成您自己的应用 id 和 key。


## 其他

如果您在使用AVOSCloud SDK中, 有自己独特高效的用法, 非常欢迎您fork 并提交pull request, 帮助其他开发者更好的使用SDK. 我们将在本项目的贡献者中, 加入您的名字和联系方式(如果您同意的话)
