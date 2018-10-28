# 内容
本文描述在信息安全课上面讲到的openssl中实践上遇到的问题

# 从源码安装
比较简单<br>
1.从官网```link：https://www.openssl.org/```上面下载最新的源码，解压，并放到虚拟机上,<br>
2.然后切换到源码的根目录下，输入```./config --prefix=/usr/local --openssldir=/usr/local/openssl```,<br>
3.继续输入```make，make test，make install```即可编译安装，到这步应该还是不会出错的<br>
4.输入```openssl```，如果显示找不到什么库，```sudo echo "（你本地的库的位置，一般是/usr/local/下有个叫lib或者lib64的，里面能够找到这个缺失的文件）" >> /etc/ld.so.conf```，然后再次输入```openssl```应该就不会出错了


aes :https://blog.csdn.net/doitsjz/article/details/50463933
