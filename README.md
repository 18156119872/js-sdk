

###wangEditor编辑器集成七牛云存储上传图片demo（js SDK） 

----

#1. wangEditor 编辑器


wangEditor——轻量级web富文本编辑器，配置方便，使用简单。支持IE8+浏览器。

* 软件官网：[wangEditor.github.io](http://wangeditor.github.io/)
* demo演示：[wangEditor.github.io](http://wangeditor.github.io/)
* 文档：[http://www.kancloud.cn/wangfupeng/wangeditor2/113961](http://www.kancloud.cn/wangfupeng/wangeditor2/113961)


#2. 使用七牛云存储

 - 七牛开发者中心：[http://developer.qiniu.com/](http://developer.qiniu.com/)
 - 七牛js sdk的下载、文档地址：[https://github.com/qiniu/js-sdk](https://github.com/qiniu/js-sdk)，该demo也是 fork 的这个项目


#3. 本地运行这个demo

第一，确定电脑已经安装了`nodejs`和`bower`。未安装的同学，请先安装这两个软件。

第二，进入[wangEditor下载页面](https://github.com/wangfupeng1988/wangEditor/releases)，下载`v2.0.14`及以上版本，解压，进入`dist`目录，得到`css`和`js`两个文件夹。待用。

第三，直接下载源码或者 `git clone https://github.com/wangfupeng1988/js-sdk.git`，下载完毕`cd js-sdk/demo/wangEditor/`进入`wangEditor`目录，将刚才下载的那`wangEditor`的`css`和`js`两个文件夹拷贝到该目录下，覆盖源文件即可。

第四，`cd ..`进入`demo`文件夹，`vim config.js`，七牛上传的一些基本参数配置一下。**注意，其中的`Uptoken_Url`默认即可，无需修改**。这一步不了解的同学，请参见[七牛js sdk使用指南](http://developer.qiniu.com/code/v6/sdk/javascript.html)

第五，`cd ..`进入`js-sdk`目录，运行`make`命令，命令运行完成之后，即可看到控制台服务启动的提示，如`Listening on port 19110`。

第六，打开浏览器，访问本地服务，例如`http://localhost:19110/wangeditor/`，不要忘了网址最后的`wangEditor`，否则你看到的将是七牛的demo页面。
