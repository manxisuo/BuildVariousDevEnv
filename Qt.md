## 1. 说明

- 操作系统版本：Windows 10 64位；
- Qt版本：5.9.9。

## 2. 准备安装文件

打开[这个链接](http://download.qt.io/official_releases/qt/5.9/5.9.9/)，下载*qt-opensource-windows-x86-5.9.9.exe*。

注：如果在Linux下，下载*qt-opensource-linux-x64-5.9.9.run*文件。

## 3. 安装

双运行安装包，按提示进行安装。需要特别注意的是，“选择组件”界面中。

首先，展开Qt -> Qt 5.9.9：

如果你希望使用MinGW进行编译，则需要选择MinGW模块；
如果你希望调用VS的编译器进行编译，则需要选择VS模块；
如果希望进行安卓开发，则需要选择安卓模块。

接下来，展开Qt -> Tools：

第一项是CDB的调试器，如果你仅使用MinGW进行编译，则此项可以不选。
第二项虽然名字带MinGW，但只是用于交叉编译的（交叉编译即在某一平台上编译用于其他平台的程序），如果用不到，也可以不选。
第三项，那是用于Perl的。如果你电脑中本身没有安装Perl，那是装不上的。

## 4. 配置

略。
