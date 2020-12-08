## Java概述与环境配置
[ day 1]
#### 1、特点

```
面向对象：用计算机模拟现实世界，解决现实问题，贴近人类思维模式

简单：不易造成内存溢出；代码可读性强

跨平台：操作系统；数据库；
	Windows
		.exe
	Linux
		.out
	macOS
		.out
	UNIX
		.out
Java因为拥有JVM，能够帮助Java程序可以支持不同的平台。
	
	(JVM:Java虚拟机)
	
Java ==> .class 字节码文件 ==> JVM在不同的平台之上给予不同解释，可以满足很多地方同时运行。

Write Once Run Anywhere
```

#### 2.编译执行和解释执行

```
编译执行是直译性语言
	C C++
	编译的结果直接交给我们的CPU运作执行，效率较高，但是不能跨平台
	
解释执行是解释性语言
	Java C#
	编译结果需要通过解释器解释之后在交给CPU执行，效率较低
	Java借助JIT技术，现在的执行效率已经接近C++
```

#### 3.JDK安装路径

```
bin
	binary二进制目录
	都是二进制可以执行文件。包含.exe文件
	java.exe
	javac.exe
	javap.exe
	javadoc.exe
db
	JDK自带的小型数据库
inclue
	系统接口目录！！！存在C写成的.h文件
jre
	Java运行环境 Java Runtime Environment
lib
	资源库目录，存在一些.jar文件 Jar包
src.zip
	Java源代码：作参考，原码思想，学习的参照物

```

#### 4.环境变量配置

```
Windows + E：打开文件资源管理器
==> 高级系统设置==> 高级==> 环境变量 ==>

系统变量（多用户）修改：

新建：
变量名：JAVA_HOME
变量值：jdk安装路径

新建：
变量名：CLASS_PATH
变量值：.;%JAVA_HOWE%\lib;%JAVA_HOME%\lib\tools.jar
(lib的相对JAVA_PATH路径;更好的复用)

编辑：
变量名：PATH
变量值：;%JAVA_HOWE%\bin;%JAVA_HOME%\jre\bin;
(path的相对JAVA_PATH路径;更好的复用)
```

#### 5.DOS命令

```
# 开启命令提示符
	Windows + R 输cmd
	
dir
# 查看当前工作目录的所有文件和文件夹

cd
# 切换工作目录
# 格式：cd 路径
# 路径唯一时tab自动补齐
# 路径【小重点】
# 相对路径
# 参照性
# . 当前工作目录
# .. 当前工作目录的父目录
# 绝对路径
# 唯一性

mkdir
# 创建文件夹
# 格式：mkdir 文件夹名（加[空格]创建多个文件夹）

rd
# 删除文件夹
# 【注意事项】
# 1.慎用 粉碎性删除
# 2.无法删除非空文件夹

echo
# [了解]
# 格式：echo [内容] > [文件名及后缀]
# 若无该文件则新建并写入/覆盖内容

# 文件扩展名 文件后缀名【重点】
# 涉及到文件操作，一定要带有文件后缀名，没有后缀名的文件电脑并不认识（解释无能）
# 第一源动力->使人“无所不能” 问题/动手/阅读/搜索/

del
# 删除普通文件，必须带文件后缀名
# 【注意事项】
# 1.慎用 直接抹掉数据

方向键上下
# 回顾之前命令

*
# 通配符，匹配

cls
# 清理窗口（但不清空缓存，还可以回顾之前命令）

exit
# 推出终端
# 后期操作某些软件为了避免不必要的麻烦

```

#### 6.要求

```
程序员一般性要求：英文字母 200APM
```



#### *名词解释

```
JVM (Java Virtyal Machine)虚拟机：
	使用软件在不同操作系统中，模拟相同的环境
JRE (Java Runtime Environment)运行环境：
	包含JVM和解释器
JDK (Java Development Kit)开发环境：
	包含JRE + 类库 + 开发工具包（编译器+调试环境）
	
```

