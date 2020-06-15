## 1. 说明

- 操作系统版本：Windows 10 64位；

## 2. 准备安装文件

- 打开[这个链接](https://flutter.dev/docs/get-started/install/windows)或[这个链接](https://flutter.cn/docs/get-started/install/windows)，下载安装包，例如*flutter_windows_1.17.3-stable.zip*。



## 3. 安装和配置Flutter

- 将压缩包解压，然后把其中的flutter目录整个放在你预想的Flutter SDK安装目录中（比如；*D:\Program\flutter*请勿将该目录放在一些需要额外操作权限的目录，比如 *C:\Program Files*）。

- 找到 flutter 目录中的*flutter_console.bat*文件，双击执行该批处理脚本。

- 打开命令行窗口，cd 到你想安装 Flutter SDK 的目录（比如*D:\Program\flutter*）。
运行以下`git clone`命令安装稳定构建渠道的 Flutter SDK。

```
git clone -b stable https://github.com/flutter/flutter.git
git clone -b stable git@github.com:flutter/flutter.git
```

注意：以上两条命令选其中一个即可，但是如果为Git设置了HTTP代理，则需要用第一条命令。

现在你可以在控制台当中使用`flutter`命令了。

如果你想要在普通的Windows控制台中使用`flutter`命令，需要将*flutter\bin*目录的完整路径加入到`PATH`环境变量。

在中国网络环境下使用 Flutter，建议设置以下环境变量：

```bash
export PUB_HOSTED_URL=https://mirrors.tuna.tsinghua.edu.cn/dart-pub
export FLUTTER_STORAGE_BASE_URL=https://mirrors.tuna.tsinghua.edu.cn/flutter
```

## 4. 运行 flutter doctor

在将 Path 变量更新后，打开一个新的控制台窗口，然后将下面的命令输入进去执行。如果它提示有任何的平台相关依赖，那么你就需要按照指示完成这些配置：

```
flutter doctor
```

上述命令会检查你的现有环境，然后把检测结果以报告形式呈现出来。仔细阅读它显示的内容，检查是否有尚未安装的软件或是有其他的步骤需要完成（通常会以粗体呈现）。

## 5. 问题解决

### 问题1

- 描述：运行`flutter doctor`时，显示Unable to locate Android SDK。

- 解决：新建环境变量`ANDROID_HOME`，取值为SDK目录的路径，例如 *D:\Program\Android\Sdk*。

### 问题2

- 描述：运行`flutter doctor`时，显示Android licenses not accepted。
- 解决：运行命令 `flutter doctor --android-licenses`，并全部接受。显示Android license status unknown时，也可用同样的方法解决。

### 问题3

- 描述：运行`flutter doctor`时，在Android Studio下显示Flutter plugin not installed。
- 解决：在*Android Studio > File > Settings > Plugins*中安装插件Flutter，以及它依赖的Dart。

### 问题4

- 描述：新建Flutter工程后，工具条中显示no devices。
- 解决：首先要确保AVD Manager中存在虚拟机；如果仍有问题，重启Android Studio。

## 6. 参考

- <https://flutter.cn/docs/get-started/install/windows>
