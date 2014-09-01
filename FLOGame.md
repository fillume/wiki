##windows 的开发环境配置

##准备
* 最新代码所在位置为github 的TEST_LITTLE_CLIENT branch.
* 安装visual studio 2010.
* 下载pthread  pthreads-w32-2-9-1-release



##如何编译？
* visual studio 打开工程文件  
    * 位置 Fight_Land_Owner_Client_VS\FightLanderOwner\FightLanderOwner.sln

* 配置环境变量
    * cocos2d 指向cocos2d-2.1rc0-x-2.1.2-hotfix 目录
    * boost_home 指向 boost库的目录 boost_1_53_0
	* 下载pthread pthreads-w32-2-9-1-release,并添加到include 和lib目录到工程中 pthreads-w32-2-9-1-release\Pre-built.2\include
* 编译
    * 修改AndroidUtil.h 中的文件
	   
    /*if(CC_TARGET_PLATFORM==CC_PLATFORM_ANDROID)
    include "platform/android/jni/JniHelper.h"
    include <android/log.h>
    endif
    */
	
   * 编译完成后debug,Resource打包到一起



	
	