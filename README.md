
错误一：
tried to access method com.google.common.base.Stopwatch.
解决：
把hadoop版本换成2.7以上

错误二：
object volatilebyteref does not have a member create
解决：
scala依赖和实际使用的scala版本不一致，换成一致的。如果无效，点击“Run”菜单，在Edit Configuration 里面，把build设为：
build， no error check。

错误三：
提示没有winutils。
解决：下载winutils。
（1）先下载对应版本的hadoop源码包，解压到本地D盘。
（2）在：https://github.com/zhouyang-bigdata/winutils
的bin/中找到对应版本的winutils.exe
（3）将winutils.exe文件放到下载的hadoop的bin目录下面。然后，创建系统环境变量HADOOP_HOME,填写hadoop路径；再在系统变量Path
里面，将HADOOP_HOME加进去，重启电脑。
