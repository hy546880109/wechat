# 微信好友扫描
python + appium 实现微信自动检测出非好友名单，运行过程可能会在通讯录界面停止则需要手动下滑一下，原因是未识别到最后一个好友界面，需要手动下滑一下帮助识别。
运行的是真机小米9，需要按自己的实际场景运行的请自行修改如下配置信息：
需要已经登陆好微信账号再运行。

优化：对不同设备的兼容，可以让用户输入不同设备的名称和版本进行兼容。（只需修改不同的系统版本号）
desired_caps = {
    "platformName": "Android",  # 系统
    "platformVersion": "10.0",  # 系统版本号
    "deviceName": "b68548ed",  # 设备名
    "appPackage": "com.tencent.mm",  # 包名
    "appActivity": ".ui.LauncherUI",  # app 启动时主 Activity
    'unicodeKeyboard': True,  # 使用自带输入法
    'noReset': True  # 保留 session 信息，可以避免重新登录
}

1.Appium环境搭建
环境搭建这里不再介绍，需要的可以看我之前的文章或者百度

2.连接真机或模拟器

3.登陆微信

4.运行程序

原文链接地址：[Python自动扫描出微信不是好友名单 - Huny - 博客园 (cnblogs.com)](https://www.cnblogs.com/huny/p/14788006.html)

