安装方法
1.将knowledge目录下的所有xml和km文件拷贝到BPPMIS所在机器上Patrol的Patrol3/lib/knowledge目录
2.将connect文件拷贝到/patrol/Patrol3/bin目录下，并执行chmod +x connect
3.将portList.txt文件拷贝到/patrol/Patrol3/PPM/Conf/目录下，注意patrol用户要有读取权限
4.patrol central端load & preload APP_PORT.km、APP.km与APP_PORT_MONITOR.km
5.更新portList.txt中的内容，增加port监控，格式如下：
第一列为目标服务器的IP地址，第二列为目标服务器的端口号，第三列为tcp,中间以逗号分隔，默认端口监控2分钟采集一次。
10.232.57.163,22,tcp