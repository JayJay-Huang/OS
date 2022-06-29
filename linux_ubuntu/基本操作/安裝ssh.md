https://www.jinnsblog.com/2020/11/linux-ubuntu-offline-install-package.html

----

# 看ubuntu版本
cat /etc/issue

# 檢查有無安裝
sudo ps -e |grep ssh

# 啟用
sudo service ssh start

# 線上安裝
sudo apt-get install openssh-server

# 檢視ip
ifconfig -a

# 網路檢測
ping [ip]

# 檢視apt-get參數
apt-get -h

# 檢視所有已安裝
sudo apt list --installed
sudo dpkg-query -l

# 檢視特定已安裝
sudo apt list --installed | grep [軟體包]
sudo dpkg-query -l | grep [軟體包]
sudo apt-get -s install [軟體包]

----
# 官網下載deb安裝包
https://packages.ubuntu.com/
搜尋 openssh-server
> https://packages.ubuntu.com/impish/openssh-server

-------
sudo apt-get install openssh-server
sudo dpkg-query -l | grep ssh
sudo mkdir offlinePackage
mkdir opensshcp /var/cache/apt/archives opensshsudo chmod 777 -R openssh

