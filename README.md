# mentohust_sourcecode

sudo apt-get install libpcap-dev autotools-dev libgtk2.0-dev libscim-dev libtool automake1.9

把mentohust解压后的文件夹（可以在树莓派上解压，也可以在windows下解压）放到树莓派的home/pi下面,
进入mentohust所在文件夹（如果在winodws下解压的话，上传到树莓派，那么还要修改一下权限 chmod 755 *）之后执行
./configure --prefix=/usr
make
sudo make install

在/usr/bin/目录下可以找到mentohust这个文件 find /usr/bin mentohust
然后给与他SUID权限，让用户都可以以root权限执行
sudo chmod u+s /usr/bin/mentohust
做完一切，shell下直接输入mentohust就可以运行了
初次执行可以能要设置一下参数，帐号，密码，网卡，等
