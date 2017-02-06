title: 在App中集成NMSSH
date: 2015-04-08 10:21:30
tags:
---

ok

前阵子淘了一块主板，挂了两块硬盘，跑个ubuntu当家庭媒体服务器用。因为不是经常用，所以有时候想把它关了，于是每次只能打开电脑，ssh连上去，“sudo shutdown -h now“，然后再关笔记本，好不繁琐~~

<!--more-->

索性写个app，来个一键关机吧~~

iOS集成ssh的资料不多，找到个[NMSSH](https://github.com/eugenehp/NMSSH)，感觉挺好用的。

NMSSH是用pod维护的，整起：

##1. 创建一个iOS工程，在命令行下进入工程目录

```shell
$cd <your project directory>
```
	
##2. 创建Podfile，内容如下：

```
platform :ios, '7.1'
pod 'NMSSH'
```

##3. 在工程目录下执行

```shell
pod install
``` 
	
安装NMSSH相关的第三方依赖

##4. 在项目中需要添加ssh逻辑的viewController.m中添加头文件

```
#import <NMSSH/NMSSH.h>
```
	
添加关机代码到- (IBAction)shutdown中：
	
```objective-c
	NMSSHSession *session = [NMSSHSession connectToHost:@"192.168.2.2:22"
	                                       withUsername:@"root"];

	if (session.isConnected) {
	    [session authenticateByPassword:@"xxx"];

	    if (session.isAuthorized) {
	        NSLog(@"Authentication succeeded");
	    }
	}

	NSError *error = nil;
	NSString *response = [session.channel execute:@"shutdown -h now" 
											error:&error];
	
	NSLog(@"Response: %@", response);

	[session disconnect];
	
```

##5. 搞定。