#我在coding路途中的那些地雷和排雷

----------
2019/12/20

一、Anaconda使用conda安装pytorch包(pytorch官网生成的链接)，收到报错提示说“无法定位程序输入点OPENSSL_sk_new_reserve于动态链接库”。

解决办法：参考[无法定位程序输入点OPENSSL_sk_new_reserve问题](https://blog.csdn.net/qq_37465638/article/details/100071259 ""https://blog.csdn.net/qq_37465638/article/details/100071259")。

操作方法：

1. 进入Anaconda\DLLS目录，查看libssl-1_1-x64.dll的日期；
1. 进入Anaconda\Library\bin目录，比较两者日期；
1. 如果不一致，将DLLS中的替换bin中的。完成。

二、使用setup.py

1. 打开cmd
1. 到达安装目录
1. python setup.py build
1. python setup.py install

或者

1. 打开cmd
1. 到达安装目录
1. pip install.

三、提示版本不对，那就安装之前的版本的包就行了。

## Mac系统

### 安装brew

时间：2021年1月26日

/bin/zsh -c "$(curl -fsSL https://gitee.com/cunkai/HomebrewCN/raw/master/Homebrew.sh)"

### 解决texstudio内置PDF不显示中文
环境 i3-4170黑苹果
终端输入

ln -s /System/Library/Fonts/Supplemental/Songti.ttc /Library/Fonts/Songti.ttc

即可解决
