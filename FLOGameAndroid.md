##android 的开发环境配置

##准备
* 最新代码所在位置为github 的TEST_LITTLE_CLIENT branch.
* 在Documents目录下新建COCOS2D_HOME目录,下载并解压cocos2d-x 2.2.2到此目录,在cocos2d-x-2.2.2/tools/project-creater 目录下运行 ./create_project.py -project FLO_Android -package com.fillume.flo -language cpp
* 在Documents目录下新建ANDROID_NDK_HOME目录,复制android-ndk-r8e
* 新建 CHINA_MOBILE_SDK目录,将移动开发包复制到此目录
* 修改.bash_profile 添加export PATH=/Users/fillume/Documents/ANDROID_NDK_HOME/android-ndk-r8e/toolchains/arm-linux-androideabi-4.7/prebuilt/darwin-x86/bin:/Users/fillume/Documents/workspace/android-sdk-macosx/platform-tools:$PATH
* 将fightland_src.zip 解压并覆盖到flo_android,有FLO_Android, floret, IOS_Ref 三个目录， 打开FLO_Android下面的用Xcode

##如何编译？
* 进入~/Documents/COCOS2D_HOME/cocos2d-x-2.2.2/projects/FLO_Android/目录,在proj.android目录下运行build_native.sh,生成libgame.so到libs/armeabi/中
* 复制CHINA_MOBILE_SDK libs中的libmegjb.so到libs/armeabi中。复制assets到assets中
* 打开eclipse生成apk

##协议变更
* 生成的协议AppProtocol目录中将所有 ">>("改成"> >("

