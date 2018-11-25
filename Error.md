react开发时用cnpm start 报错：原因是LINUX系统文件数量限制

https://www.len168.com/article/detail.html?id=9

解决方法：

echo fs.inotify.max_user_watches=524288 | sudo tee -a /etc/sysctl.conf && sudo sysctl -p
