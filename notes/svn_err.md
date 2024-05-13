1）命令找到对应项目的目录中的.svn文件目录（该文件默认隐藏，修改属性进行显示），并查看是否存在wc.db文件；(E:\svn\yykj\.svn)

2）输入：sqlite3 wc.db    进入wc.db文件；

3）输入：.table    查看文件的信息（注意table前面有点），会有work_queue表；

4）输入：sqlites3 select * from work_queue;    查看到对应锁定的文件信息；

5）输入：sqlite3 delete from work_queue;     即可解除锁定的文件。

6）完成