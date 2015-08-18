# ZhangYouBaoServer
掌邮宝服务器端

具体配置方法如下：(windows端下开发，开发完成后移植到linux平台)
（过程中涉及的所有安装资源以共享到http://pan.baidu.com/s/1pJnAv0J，请自行下载）


1.安装最新版wampserver(由于ThinkPHP要求php版本要高于5.3，最新的wamp php版本为5.5)


2.删去wamp安装后www目录下的所有文件，并解压thinkPHP框架到该文件夹下


3.在www的上一层目录建立文件夹，如本人建立develop目录，并修改thinkPHP默认入口index.php文件如下：

// 定义应用目录
define('APP_PATH','../develope/Application/');

// 引入ThinkPHP入口文件
require '../develope/ThinkPHP/ThinkPHP.php';

4.直接删去thinkPHP框架中的application和thinkPHP文件夹

5.将从本仓库中pull到的内容复制到上文中建立的develop目录下

6.安装zend studio进行php开发，打开develop文件夹即可进行开发

7.具体thinkPHP框架使用方法请查阅http://www.thinkphp.cn/ 下开发手册

注：window下提交的时候github可能会出现warning: LF will be replaced by CRLF的提示，我这边是执行 git config --global core.autocrlf false  //禁用自动转换    