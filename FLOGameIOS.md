##IOS 的开发环境配置

##准备
* 最新代码所在位置为github 的TEST_LITTLE_CLIENT branch.
* 在Documents目录下新建COCOS2D_HOME目录,下载并解压cocos2d-x 2.2.2到此目录,在cocos2d-x-2.2.2/tools/project-creater 目录下运行 ./create_project.py -project FLO_Android -package com.fillume.flo -language cpp
* 在Documents目录下新建ANDROID_NDK_HOME目录,复制android-ndk-r8e
* 修改.bash_profile 添加export PATH=/Users/fillume/Documents/ANDROID_NDK_HOME/android-ndk-r8e/toolchains/arm-linux-androideabi-4.7/prebuilt/darwin-x86/bin:/Users/fillume/Documents/workspace/android-sdk-macosx/platform-tools:$PATH
* 将fightland_src.zip 解压并覆盖到flo_android,有FLO_Android, floret, IOS_Ref 三个目录， 打开FLO_Android下面的用Xcode

##如何编译？
* 修改build setting中的lib, header路径
* 编译运行

* 进入~/Documents/COCOS2D_HOME/cocos2d-x-2.2.2/projects/FLO_Android/目录,在proj.android目录下运行build_native.sh

* 配置环境变量
    * cocos2d 指向cocos2d-2.1rc0-x-2.1.2-hotfix 目录
    * boost_home 指向 boost库的目录 boost_1_53_0
	* 下载pthread pthreads-w32-2-9-1-release,并添加到include 和lib目录到工程中 pthreads-w32-2-9-1-release\Pre-built.2\include
* 编译
    * 修改AndroidUtil.h 中的文件
	```/*if(CC_TARGET_PLATFORM==CC_PLATFORM_ANDROID)

include "platform/android/jni/JniHelper.h"

include <android/log.h>

endif

*/
```
   * 编译完成后debug,Resource打包到一起
