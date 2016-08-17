如何搭建：
react-native
react-web

//windows配置react-native:
安装JDK
安装nodejs
安装python（C++环境）
npm install -g react-native
npm install -g react-native-cli
//adb安装Apk
一、配置系统环境变量：
ANDROID_HOME：E:\android-sdk//sdk的安装目录
在path中加入：;%ANDROID_HOME%\tools;%ANDROID_HOME%\platform-tools
//创建项目
react-native init X
react-native start
react-native run-android
*首次运行会出现红色错误页面，安卓设备按菜单键在Dev Settings中设置服务器ip和端口
重新加载页面就OK
react-native 智能提醒：（webstorm：file->import setting->ReactNative.jar）
git clone https://github.com/virtoolswebplayer/ReactNative-LiveTemplate

参考文档：
http://facebook.github.io/react-native/releases/0.31/docs/webview.html#webview
http://www.kancloud.cn/digest/rnative/121808