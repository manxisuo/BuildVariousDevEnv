## 1. 说明

- 操作系统版本：Windows 10 64位；
- Java版本：8u251。

## 2. 准备安装文件

打开[这个链接](https://www.oracle.com/java/technologies/javase/javase-jdk8-downloads.html)，下载jdk-8u251-windows-x64.exe。

## 3. 安装

双运行安装包，按提示进行安装。

## 4. 配置

- 建立系统环境变量`JAVA_HOME`，取值为`C:\Program Files\Java\jdk1.8.0_251`；
- 修改系统环境变量`PATH`，加入`%JAVA_HOME%\bin`。


## 5. 测试

在cmd中分别执行`java`和`javac`命令，能够正常输出，说明安装和配置成功。
