# Sencha Cmd安装笔记

###sencha Cmd 提供了一系列功能强大的节约时间的功能，结合Sencha Ext JS 和Sencha Touch框架协同工作。Sencha Cmd 提供了如下几个能力：

1. 代码生成工具：代码生成工具生成整个应用程序并且扩展生成mvc的组件框架，如，使用sencha generate app 命令，可以自动帮你生成一个完成的应用程序目录框架。
2. JS编译:框架意识，Javascript 编译器了解Sencha的语义语法，并且从你源代码构建的时候产生较少的足迹。编译器通过Sencha框架减少加载应用程序的时间来优化高层次的语义。
3. 网络服务：提供了轻量级的网络服务，如，使用sencha web start 可以启动网络服务。
4. 本地包装：以一流的移动应用程序访问设备给移动应用程序并且可以方便的分布到移动商店。
5. 包装管理系统：方便集成的由管理系统(像Ext js 的主题)
6. 构建脚本. 通过在应用程序中增加“before”和"after"给应用程序增加一些额外的设置点让客户可以定制适合自己需求的脚本。
7. 转换工具：强大的代码选择器转换你项目中需要最终构建需要的代码，决定页面和局部共享代码的高级别选择集像你需要的那样构造。
8. 工作空间管理：过不同的应用程序共享框架工作，包河自定义的代码透。
9. 图像提取：转换CSS3的特性（比如边界半径和线性梯度）
10. 灵活的配置系统： 在一台机器上允许命令行操作程序或者在工作空间级别或者整个工作空间。
11. 日记功能：强大的日志功能帮助你理解整个内部的命令行工作，排除故障。
12. 三方控件： Sencha cmd 包含了Compass sass 和ant 。
13. 代码生成的钩子：可以指定到一个页面或者在工作控件分享所有页面，例如检查daunting的惯例或者产生新的模型。

## 兼容性

> Sencha Cmd 支持Sencha Ext JS 的4.1.1a以及以上版本还有Sencha Touch的2.1版本以及以上，许多的新功能需要在框架的支持下工作，都是可以使用的版本。

> 对旧版本来说，有些低级命令式可以使用的。

> 如果你在使用旧版本的Ext JS 你可以使用Sencha Cmd的build命令来构造你的JSB文件。换句话说，Sencha Cmd 可以将JSB文件生成压缩的构造包来替换之前版本，这操作不会更新你的那些有之前SDK生成的JSB文件。

> Sencha Touch2.0和Sencha Ext JS 4.0 需要SDK2.0版本的工具，在以后的版本中是不会被支持的哦。


    Sencha Cmd下载地址：https://www.sencha.com/products/extjs/cmd-download/
    Sencha Cmd 6官网地址：http://docs.sencha.com/cmd/6.x/
    Sencha Cmd 6相关细节的地址：http://docs.sencha.com/cmd/6.x/cmd_upgrade_guide.html
    
## 安装sencha CMD

1. jdk安装
2. 安装ruby
3. 安装secha cmd
    安装过程中，会提示是否兼容以前版本（如下图），勾选后则兼容6以前的版本，如果安装以前的老版本，则不存在这种问题。
![tupian][1]
4. 开命令行 即CMD 切换到安装目录下，输入 sencha命令，查看是否安装成功
5. 更新sencha Cmd 执行命令 sencha upgrade --check
6. sencha help 查看sencha 基本命令

> encha cmd 6安装过程不需要UAC控制了对于widnows来说，对于mac来说是启动权限，之前的版本，我们比较麻烦的事情是需要下载正确的ruby版本才可以使用cmd，现在6.0版本之后，就不需要单独安装ruby了，新版取消了对ruby的依赖。新版cmd增加了对jre的默认安装，选择下载包的时候，可以直接下载带有jre的安装包，这样就不需要再单独安装jre啦，这对不熟悉java安装环境的用户来说，又是一大福利。对于编译的compass扩展，新版也做了改进，如果是不是再使用旧版本，则，可以不再安装compass extension了。

## 应用

1. 生成应用程序

    sencha generate app -ext MyApp E:\senchaworkspace\MyApp
    需要注意的是，生成的EXTjs 是商业体验版本，
    如果你购买了，那么你需要下载extjs的zip包，并且使用-SDK命令来制定SDK的路径，这样，就不会去默认下载SDK而是按照你本地的文件来生成了。命令如下： 
    sencha -sdk /这里是你的sdk路径/ generate app MyApp 你的App的路径。如 sencha -sdk c:sencha5.0.0 generate app OASystem d:\oasys
    
2. 


[1]:http://images0.cnblogs.com/blog2015/249616/201507/030102266926108.png
