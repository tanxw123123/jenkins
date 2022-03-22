安装  
环境：ubuntu 20.04  

1. 安装java  
```
$ sudo apt update
$ sudo apt install openjdk-11-jdk
$ java -version
```

2. 安装
官网地址：<https://www.jenkins.io/doc/book/installing/linux/#debianubuntu>
```
$ curl -fsSL https://pkg.jenkins.io/debian-stable/jenkins.io.key | sudo tee \
  /usr/share/keyrings/jenkins-keyring.asc > /dev/null
$ echo deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc] \
  https://pkg.jenkins.io/debian-stable binary/ | sudo tee \
  /etc/apt/sources.list.d/jenkins.list > /dev/null
$ sudo apt-get update
$ sudo apt-get install jenkins
```
访问：http://ip:8080  

3. 卸载  
```
$ sudo apt remove jenkins                 #服务
$ sudo apt remove --auto-remove jenkins   #安装包
$ sudo apt purge jenkins                  #配置数据
$ sudo apt purge --auto-remove jenkins    #配置数据

```
