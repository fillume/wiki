##IOS �Ŀ�����������

##׼��
* ���´�������λ��Ϊgithub ��TEST_LITTLE_CLIENT branch.
* ��DocumentsĿ¼���½�COCOS2D_HOMEĿ¼,���ز���ѹcocos2d-x 2.2.2����Ŀ¼,��cocos2d-x-2.2.2/tools/project-creater Ŀ¼������ ./create_project.py -project FLO_Android -package com.fillume.flo -language cpp
* ��DocumentsĿ¼���½�ANDROID_NDK_HOMEĿ¼,����android-ndk-r8e
* �޸�.bash_profile ���export PATH=/Users/fillume/Documents/ANDROID_NDK_HOME/android-ndk-r8e/toolchains/arm-linux-androideabi-4.7/prebuilt/darwin-x86/bin:/Users/fillume/Documents/workspace/android-sdk-macosx/platform-tools:$PATH
* ��fightland_src.zip ��ѹ�����ǵ�flo_android,��FLO_Android, floret, IOS_Ref ����Ŀ¼�� ��FLO_Android�������Xcode

##��α��룿
* �޸�build setting�е�lib, header·��
* ��������

* ����~/Documents/COCOS2D_HOME/cocos2d-x-2.2.2/projects/FLO_Android/Ŀ¼,��proj.androidĿ¼������build_native.sh

* ���û�������
    * cocos2d ָ��cocos2d-2.1rc0-x-2.1.2-hotfix Ŀ¼
    * boost_home ָ�� boost���Ŀ¼ boost_1_53_0
	* ����pthread pthreads-w32-2-9-1-release,����ӵ�include ��libĿ¼�������� pthreads-w32-2-9-1-release\Pre-built.2\include
* ����
    * �޸�AndroidUtil.h �е��ļ�
	   /*if(CC_TARGET_PLATFORM==CC_PLATFORM_ANDROID)

include "platform/android/jni/JniHelper.h"

include <android/log.h>

endif

*/
   * ������ɺ�debug,Resource�����һ��
