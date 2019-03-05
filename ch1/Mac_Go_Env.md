# Mac环境配置

## 下载
链接：https://golang.google.cn/dl/

## 安装
双击下载后的dmg进行安装，安装成功后，打开终端，输入下面命令查看是否安装成功：
```
> go version
```

显示如下：
```
RickydeMacBook-Pro:~ apple$ go version
go version go1.12 darwin/amd64
```
那么恭喜你，安装成功。

## 环境变量配置
步骤如下：
* 打开终端，cd ~进入主目录
* ls -all查看所有文件，看是否存在.bash_profile文件
* 如果不存在，则执行touch .bash_profile新建
* 如果存在，则执行vi .bash_profile打开进行编辑

在文件中添加如下参数：
```
export GOPATH=/Users/apple/Ricky/go
export GOBIN=$GOPATH/bin
export PATH=$PATH:$GOBIN
```

使修改立刻生效:
```
source .bash_profile
```
