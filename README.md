# 关于adb的交叉编译

本项目是用来编译adb使用的，因为存在可能有非常规架构cpu的linux系统需要使用adb，因此从大佬那边fork这个项目修修改改来食用

本项目已经继承了一些必要的编译需要的东西，然后可能需要安装专属的gcc g++这些库

### 1、克隆项目

```bash
git clone https://github.com/SilverIceKey/adb-cross-compile.git
```

### 2、进入adb目录

```bash
cd adb-cross-compile
cd system/core/adb
```

### 3、编译

因为已经配置好了Makefile，所以可以直接执行编译命令

```bash
make //编译完成之后，所在目录下面会有adb的二进制文件
make install //将adb的二进制文件复制到/usr/bin
```

至此编译就完成了。感谢使用！