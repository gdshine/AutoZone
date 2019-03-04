# AutoZone
web，APP ，接口 UI自动化一体测试平台
测试平台解决了web，app部分元素无法定位的痛点，只需要对无法定位的点进行截图，然后上传到工程目录下后，在自动化用例里面输入图片的名称与格式就会进行图像的匹配识别，识别到后会完成点击与判断页面是否存在等操作
开发测试平台的初衷：希望web,app的UI自动化和接口的自动化能够一起执行，去掉jenkins构建，代码重构，繁多等问题。
本平台是1.0版本，后续还将完善更多的功能（考虑是作成一个测试的客户端还是网页）

什么是AutoLine开源平台
Autotime开源平台是一个开源自动化测试解决方案，基于RobotFramework进行二次开发，支持RobotFramework几乎所有的库。并能够实现图像识别查找GUI等功能。
采用了哪些开源技术/框架
python3
Django
Bootstrap3
requests
pymysql
pyautoGUI
Pyhook
robotframework
Selenium2library
SikuliLIbrary
APSscheduler
等库与插件
如何运行
下载完整的工程文件后，pycharm中打开
运行
python manage.py runserver 指定希望运行的端口
然后在网页上输入网址比如127.0.0.1:9000/login/
登陆后页面显示如下：

ps:背景刚开始看还可以，后面越看越丑，有推荐的嘛？
创建登录的账号和密码：
pycharm Tools>Run manage.py Task ;或者直接快捷键ctrl +alt+Ｒ，然后在输入createsuperuser,创建admin,然后按照提示输入账户和密码
登陆后页面展示如下>
一些截图



接口参数添加页面如下
Assert 中可以对多个参数做判断（后续将增加对返回值参数是否存在与数据库中的断言）
测试报告如下

Web自动化
web自动化步骤的添加和robotframework的一样，区别是增加了填写的参数位置固定了。步骤添加页面设计来源于Django 自带的admin模板 +suit这个美化过


支持关键字蓝色高亮显示

只需将需要点击的图标截图名称填写进步骤里面

图片上传的路径平台已做设定，选择上传就可以了。注：图片识别并点击截图，需要如下的截图才能识别—



等，图片背景变换会导致识别不到对应的截图，所以要保持点击的图标背景与截图的一致
所有测试用例支持运行所选部分和全部，支持定时任务的执行

测试报告暂时用的robotframework的 ，后续将测试报告改的和web的测试报告一致

支持向添加到数据库的邮箱发送测试报告

web支持对应的关键字查询与说明

测试平台的基本情况 已经讲解完成，后续将讲解相应部分的代码
我的QQ:1633235633@qq.com，有问题可以联系。后续开发完后将公布github地址，进行开源以便发现更多的问题
