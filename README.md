# 安卓终端模拟器
 十年前创建的老项目了，原作者已经不再维护。由于网上直接下载的.so本地库文件也都是基于历史版本的32位库，而我需要一个64位的，因此fork了一份。
 更新了一下gradle发行版到7.3.3 android gradle 插件到7.0.4
 修改了各个模块的build.gradle文件，直接打包后支持 "arm64-v8a", "armeabi-v7a", "x86", "x86_64"
## 打包说明

- 克隆本仓库到本地
- 下载最新版AndroidStudio
- 打开本项目，将gradle插件的jdk修改为java11 因为gradle需要java11以上
- 等待gradle同步完成，点击运行 term 即可创建apk文件，默认生成的未进行签名，只需要so文件的话解压apk获取即可（我的目的就是so文件）
- 也可以通过命令行模式打包 `./gradlew clean && ./gradlew build`
- 目标apk位置为 `term/build/outputs/apk/release/term-release-unsigned.apk`


# Terminal Emulator for Android

*Note:* Terminal Emulator for Android development has ended. I am not
accepting pull requests any more.

Terminal Emulator for Android is a terminal emulator for communicating with the
built-in Android shell. It emulates a reasonably large subset of Digital
Equipment Corporation VT-100 terminal codes, so that programs like "vi", "Emacs"
and "NetHack" will display properly.

This application was previously named "Android Terminal Emulator". Same great
application, just with a new name. (The change was made at the request of the
Android trademark owner.)

This code is based on the "Term" application which is included in the Android
Open Source Project. (Which I also wrote. :-) )

[Download the Terminal Emulator for Android from Google Play](https://play.google.com/store/apps/details?id=jackpal.androidterm)

If you are unable to use the Play Store, you can also
[download from GitHub](https://jackpal.github.io/Android-Terminal-Emulator/)

See [Building](docs/Building.md) for build instructions.

Got questions? Please check out the
[FAQ](http://github.com/jackpal/Android-Terminal-Emulator/wiki/Frequently-Asked-Questions). Thanks!

Please see the
[Recent Updates](http://github.com/jackpal/Android-Terminal-Emulator/wiki/Recent-Updates)
page for recent updates.
