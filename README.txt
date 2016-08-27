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

//react-web
npm install react-web-cli -g
react-web init X-name
文档：https://github.com/taobaofed/react-web
//打包
react-web bundle

参考文档：
http://facebook.github.io/react-native/releases/0.31/docs/webview.html#webview
http://www.kancloud.cn/digest/rnative/121808
http://blog.csdn.net/watertekhqx/article/details/51302235

Flex布局
http://www.tuicool.com/articles/a6Rjmi2
 
所有属性：
"alignItems",
"alignSelf",
"backfaceVisibility",
"backgroundColor",
"borderBottomColor",
"borderBottomLeftRadius",
"borderBottomRightRadius",
"borderBottomWidth",
"borderColor",
"borderLeftColor",
"borderLeftWidth",
"borderRadius",
"borderRightColor",
"borderRightWidth",
"borderStyle",
"borderTopColor",
"borderTopLeftRadius",
"borderTopRightRadius",
"borderTopWidth",
"borderWidth",
"bottom",
"color",
"flex",
"flexDirection",
"flexWrap",
"fontFamily",
"fontSize",
"fontStyle",
"fontWeight",
"height",
"justifyContent",
"left",
"letterSpacing",
"lineHeight",
"margin",
"marginBottom",
"marginHorizontal",
"marginLeft",
"marginRight",
"marginTop",
"marginVertical",
"opacity",
"overflow",
"padding",
"paddingBottom",
"paddingHorizontal",
"paddingLeft",
"paddingRight",
"paddingTop",
"paddingVertical",
"position",
"resizeMode",
"right",
"rotation",
"scaleX",
"scaleY",
"shadowColor",
"shadowOffset",
"shadowOpacity",
"shadowRadius",
"textAlign",
"textDecorationColor",
"textDecorationLine",
"textDecorationStyle",
"tintColor",
"top",
"transform",
"transformMatrix",
"translateX",
"translateY",
"width",
"writingDirection"
 
 
pm2
安装：npm install -g pm2
启动程序：pm2 start <app_name|id|all>
列举进程：pm2 list
退出程序：pm2 stop <app_name|id|all>
重起应用：pm2 restart
程序信息：pm2 describe id|all
监控：pm2 monit
实时集中log处理: pm2 logs
API:pm2 web (端口：9615 )
 
pm2 cluster模式：
1. 使用-f 参数强制其更换启动模式：pm2 start app.js -i 2 -f
2. 使用pm2 kill ，关闭deamon，然后重新使用pm2 start app.js开启。
 
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
react-native 智能提醒：（webstorm：file->import setting->ReactNative.jar）
git clone https://github.com/virtoolswebplayer/ReactNative-LiveTemplate
 
参考文档：
http://facebook.github.io/react-native/releases/0.31/docs/webview.html#webview
http://www.kancloud.cn/digest/rnative/121808
https://github.com/reactnativecn/react-native-guide
https://github.com/taobaofed/react-web
 
 
打包：gradlew assembleRelease（Android目录下）
配置：在gradle.properties增加：
MYAPP_RELEASE_STORE_FILE=lyp.keystore
MYAPP_RELEASE_KEY_ALIAS=lyp
MYAPP_RELEASE_STORE_PASSWORD=password
MYAPP_RELEASE_KEY_PASSWORD=password
在android/app/build.gradle增加：
signingConfigs {
       release {
           storeFile file(MYAPP_RELEASE_STORE_FILE)
           storePassword MYAPP_RELEASE_STORE_PASSWORD
           keyAlias MYAPP_RELEASE_KEY_ALIAS
           keyPassword MYAPP_RELEASE_KEY_PASSWORD
       }
    }
   buildTypes {
       release {
           minifyEnabled enableProguardInReleaseBuilds
           proguardFiles getDefaultProguardFile("proguard-android.txt"),
"proguard-rules.pro"
           signingConfig signingConfigs.release
       }
    }
 
Adb命令：
adb kill-server
adb devices
adb install -r x.apk  //-r 强制安装
 
keytool:
 
keytool -list -keystore x.keystore
 keytool -genkeypair -alias "name" -keyalg "RSA" -keystore "name.keystore"  
 
微信开发文档：
http://mp.weixin.qq.com/wiki/7/aaa137b55fb2e0456bf8dd9148dd613f.html#.E8.8E.B7.E
 
5.8F.96.E2.80.9C.E5.88.86.E4.BA.AB.E7.BB.99.E6.9C.8B.E5.8F.8B.E2.80.9D.E6.8C.89.
 
E9.92.AE.E7.82.B9.E5.87.BB.E7.8A.B6.E6.80.81.E5.8F.8A.E8.87.AA.E5.AE.9A.E4.B9.89
 
.E5.88.86.E4.BA.AB.E5.86.85.E5.AE.B9.E6.8E.A5.E5.8F.A3
 
//ES6
http://es6.ruanyifeng.com/
 