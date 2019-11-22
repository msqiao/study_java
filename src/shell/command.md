## 一、Shell概念学习
### 1、shell是什么？
shell是连接用户和内核之间得桥梁，也可以简称是代理，也是将用户、程序、用户连接起来得。<br>
调用其他程序，给其他程序传递数据或参数，并获取程序的处理结果；<br>
在多个程序之间传递数据，把一个程序的输出作为另一个程序的输入；<br>
Shell 本身也可以被其他程序调用。
### 2、shell有哪些？
shell也是由很多组织机构去开发，也分出了好多版本也有不通得优缺点<br>
常见得shell版本有sh、bash、csh、tcsh、ash，目前bash是默认得shell兼容了sh但是也不完全包括<br>
查看Linux系统使用得shell：cat /etc/shells 	<br>
查看Linux系统默认使用shell：echo $SHELL 
### shell终端模拟包有哪些?
centos 默认使用GNOME终端<br>
比如xterm是x windows 桌面程序自带得<br>
Konsole终端整合了xterm特性及类似windows得高级特性
### shell命令集合？
echo 输出命令，可以输出数字、变量、字符串等，格式 echo "Java语言" 或者 echo " java 语言 " （先输入" 之后内容 之后 ")
### shell 第一个脚本？
#！/bin/bash  --> # 表示注释 #！约定标记表明什么解释器执行 /bin/bash 解释器得具体位置<br>
read PERSON --> read 标准输入文件，读取用户输入得数据<br>
echo "Hello $PERSON" --> $PERSON 输出遍历PERSON 内容
### shell 执行脚本方式？
source test.sh --> source 命令读取并在当前环境执行脚本<br>
sh test.sh<br>
./tesh.sh 增加执行权限 chmod +x test.sh <br>
### shell 变量得操作
### 查看进程号及位置
ps -aux | grep redis<br>
ll /proc/5393/cwd	
