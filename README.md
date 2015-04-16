## 介绍
这个是一个演示反馈功能用法的示例项目。

![feedback](https://cloud.githubusercontent.com/assets/5022872/5720118/ae309faa-9b5a-11e4-9d94-5c632089d9fe.png)

## 如何运行

你可以使用`cocoapods`,将`Frameworks`目录下的文件删除，然后在终端执行代码:

	    pod install

    不出问题的话 1分钟即可完成所有设置, 并生成名为`FeedbackDemo.xcworkspace`的Xcode工作空间，用Xcode打开它，按第1种介绍的方法运行即可

----

## 使用说明

### 替换 App 信息

示例使用的是公共的 app id 和 app key，您可以在`AppDelegate.m`修改成您自己的应用 id 和 key。

### 反馈页面无法返回怎么办

如果你的意见反馈页面出现如上图所示的界面，这时候你会发现，导航条左边的返回或者取消按钮不存在，所以会导致用户无法退出这个页面。

其实 LeanCloud Feedback 组件中默认的意见反馈页面是有一个返回按钮的，出现这个问题的原因在于 LeanCloud SDK 的资源文件没有被加载进来。你可以通过如下步骤来解决这个问题：

- 找到 ./Pods/AVOSCloud/iOS/```release-va.b.c```/AVOSCloud.framework 这个文件(这里```va.b.c```是具体的版本号，例如目前我们最新发布的是v3.0.2，所以对应的路径是```release-v3.0.2```)
- 右键点击```AVOSCloud.framework```，选择「在新窗口中打开」（或者「Open in New Tab」）
- 这时候你会看到```AVOSCloud.bundle```这个文件，将它拖到工程里面即可。


## 其他

如果您在使用AVOSCloud SDK中, 有自己独特高效的用法, 非常欢迎您fork 并提交pull request, 帮助其他开发者更好的使用SDK. 我们将在本项目的贡献者中, 加入您的名字和联系方式(如果您同意的话)
