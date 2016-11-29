#NodeJs 环境搭建
当前搭建版本： node v6.9.1 && npm 3.10.8

> nodejs的[官网](https://nodejs.org/en/)本身自带npm，所以不需要再安装一遍npm


##Linux(Centos 7.2.1511)
>注意：如果下载的是压缩包 则系统那个需要安装Python 2.6 或者 2.7 来构造

###安装环境
	
   * Python 2.6 或 2.7(构建源码包需要)
   
   * GCC && G++ 4.2 or newer
   
### 安装步骤
1. 下载源码到 **/usr/src/node** （目录名称可以自定义）
    
    `wget https://nodejs.org/dist/v6.9.1/node-v6.9.1-linux-x64.tar.xz`

	*linux下载的时候报错,所以直接从网页端下载linux版的[node安装包](https://nodejs.org/dist/v6.9.1/node-v6.9.1-linux-x64.tar.xz)然后拷到linux系统上*

2. 解压

    `cd node-v6.9.1-linux-x64`<br/>
    `tar -xf node-v6.9.1-linux-x64`
	
3.  建立软连接（为了可以全局使用node）
	
    `ln -s /usr/src/yanjiao/node-v6.9.1-linux-x64/bin/node  /usr/local/bin/node`<br/>
    
    `ln -s /usr/src/yanjiao/node-v6.9.1-linux-x64/lib/node_modules/npm/bin/npm-cli.js /usr/local/bin/npm`

4.  测试
	
	`node -v`<br/>
	`npm -v`

测试可以正常输出版本号，这样linux版本的node就安装好了

##windows(windows 8)
windows更简单 直接在官网上下载windows版的[node安装包](https://nodejs.org/dist/v6.9.1/node-v6.9.1-x64.msi)	
