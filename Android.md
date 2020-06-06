## 1. 说明

- 操作系统版本：Windows 10 64位；
- Java版本：8u251。

## 2. 准备安装文件

打开[这个链接](https://developer.android.google.cn/studio)，下载安装包，例如*android-studio-ide-193.6514223-windows.exe*。

## 3. 安装

双运行安装包，按提示进行安装。

注：如果要彻底卸载Android，需删除`%USERPROFILE%`下面的 *.android* 和 *.ndroidStudio4.0* 或者类似名称的目录。

## 4. 配置

首次运行时，进行初始配置。例如：选择JDK（Gradle构建工程时使用）的路径、选择安装的组件（Android SDK和AVD等）。

~~为了正常下载，建议设置国内源（代理），例如：东软信息学院的 mirrors.neusoft.edu.cn ，端口80。~~

首次运行时，如果不能正常连接，会跳出设置代理的界面。注意：首次运行时不要设置代理。

后续配置代理的步骤：File -> Setting -> System Settings -> HTTP Proxy

## 5. 测试

XXX

## 6. 问题解决

### 问题1

- 描述：在AVD Manager中启动模拟器时，报错 unable to locate adb。
- 解决：**未知**

### 问题2

- 描述：Gradle如何设置代理。
- 解决：参考<https://stackoverflow.com/questions/31668234/android-studio-gradle-proxy-settings>。