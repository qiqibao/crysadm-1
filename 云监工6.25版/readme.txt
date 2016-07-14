整合包，提供config.py文件的模板:config.py.template。请修改SECREAT_KEY字段后改名使用

内置了update.sh。
update.sh依赖unzip软件包，如果没有运行：su -c root 'apt-get install unzip' 安装
升级流程为：
1.下载源码包，命名为crysadm.zip
2.上传到服务器的监工路径下的tmp目录
3.运行update.sh
脚本会自动解压升级包。并将旧版本备份到crysadm.old
