# 0. Android 工具
- dumpsys   
   - AndroidDeveloper官网 https://developer.android.com/studio/command-line/dumpsys   
- gradle
   - dependencies
      - Android Studio3.0中dependencies依赖由compile变为implementation的区别 https://blog.csdn.net/SilenceOO/article/details/78735687

# 1. performance
## (0) General
- 理论
   - AndroidDeveloper官网-Performance tips https://developer.android.com/training/articles/perf-tips
- 工具
   - fish-Android性能检测工具 https://zhuanlan.zhihu.com/p/31828854

## (1) ANR
- AndroidDeveloper官网-Keeping your app responsive https://developer.android.com/training/articles/perf-anr
- gityuan-Input系统—ANR原理分析(原理) http://gityuan.com/2017/01/01/input-anr/
- duanqz-ANR机制以及问题分析(原理+实战) http://duanqz.github.io/2015-10-12-ANR-Analysis

## (2) RAM
- 工具
   - AndroidDeveloper官网-[AS 3.0以前]Memory Monitor https://developer.android.com/studio/profile/am-memory 
- 视频
   - 阿里巴巴-Android内存优化 http://www.infoq.com/cn/presentations/android-memory-optimization
- 理论
   - AndroidDeveloper官网-Overview of memory management https://developer.android.com/topic/performance/memory-overview
   - AndroidDeveloper官网-Manage your app's memory https://developer.android.com/topic/performance/memory
   - AndroidDeveloper官网-调查 RAM 使用情况 https://developer.android.com/studio/profile/investigate-ram?hl=zh-cn
   - AndroidDeveloper官网-利用 Android Profiler 测量应用性能 https://developer.android.com/studio/profile/android-profiler?hl=zh-cn
   - AndroidDeveloper官网-使用 Memory Profiler 查看 Java 堆和内存分配 https://developer.android.com/studio/profile/memory-profiler?hl=zh-cn#分析内存的技巧
   - AOSP官网-调试本地内存使用 https://source.android.com/devices/tech/debug/native-memory
   - gityuan-Android内存分析命令(内容较概括) http://gityuan.com/2016/01/02/memory-analysis-command/
   - CSDN-Android的进程回收机制 https://blog.csdn.net/hello_zhou/article/details/50250801
   - fish-Android native内存检测 https://zhuanlan.zhihu.com/p/29176806
   - hukai-Android内存优化之OOM http://hukai.me/android-performance-oom/
   - bugly-Android 内存优化总结&实践 https://mp.weixin.qq.com/s/2MsEAR9pQfMr1Sfs7cPdWQ
   - bugly-csdn-优化安卓应用内存的神秘方法以及背后的原理，一般人我不告诉他 https://blog.csdn.net/tencent_bugly/article/details/47754955
   - MAT - Memory Analyzer Tool 使用进阶 http://www.lightskystreet.com/2015/09/01/mat_usage/
   - bugly-Android 开发绕不过的坑：你的 Bitmap 究竟占多大内存？ https://mp.weixin.qq.com/s?__biz=MzA3NTYzODYzMg==&mid=403263974&idx=1&sn=b0315addbc47f3c38e65d9c633a12cd6&scene=21#wechat_redirect
   - Using the Memory Profiler tool https://google-developer-training.gitbooks.io/android-developer-advanced-course-practicals/unit-2-make-your-apps-fast-and-small/lesson-4-performance/4-2-p-memory-profiler/4-2-p-memory-profiler.html
   - Android 内存分析 https://blog.csdn.net/heng615975867/article/details/51259410
   - bugly-腾讯优测-如何降低App的待机内存：
      1. 越用越卡为哪般——如何降低App的待机内存 https://blog.csdn.net/Tencent_Bugly/article/details/53464096
      2. 规范测试流程及常见问题 https://blog.csdn.net/tencent_bugly/article/details/53583768
      3. 探索内存增长的原因 https://blog.csdn.net/Tencent_Bugly/article/details/53740748
      4. 进阶：内存原理 https://blog.csdn.net/Tencent_Bugly/article/details/53994286
      5. 优化dex相关内存及本章总结 https://blog.csdn.net/Tencent_Bugly/article/details/54287565
   
- 原理
   - LeakCanary:
      - LeakCanary 内存泄露监测原理研究 https://www.jianshu.com/p/5ee6b471970e
      - fish-LeakCanary原理解析 https://zhuanlan.zhihu.com/p/34672399
- 实例
   - wetest-LeakCanary+Jenkins内存泄漏监控实践 http://wetest.qq.com/lab/view/175.html
   - wetest-专项：Android 内存泄露实践分析 http://wetest.qq.com/lab/view/161.html
   - Qzone-Android 内存泄漏分析心得 https://blog.csdn.net/tencent_bugly/article/details/54668776

## (3) launch-time 
- 理论
   - AndroidDeveloper官网-App Startup Time https://developer.android.com/topic/performance/vitals/launch-time

## (4) apk-size
- bugly-【译】使用 APK Analyzer 分析你的 APK https://mp.weixin.qq.com/s?__biz=MzA3NTYzODYzMg==&mid=2653578947&idx=2&sn=1f46a2ad05f1583ac4f9ee1bcf5d832d&chksm=84b3b4c4b3c43dd2d891a74ee8ae938667b706ee63c618e88a38241921e205c4f1d8825a5fa0&scene=21#wechat_redirect
- bugly-Android APK 瘦身 - JOOX Music项目实战 https://blog.csdn.net/tencent_bugly/article/details/71404513
- bugly-Android减包-减少APK大小 https://blog.csdn.net/tencent_bugly/article/details/71165675
- bugly-weixin 安装包立减1M--微信Android资源混淆打包工具 https://mp.weixin.qq.com/s?__biz=MzA3NTYzODYzMg==&mid=214472913&idx=1&sn=92b54b5fcd9bbab6513e46d92095a07f&scene=21#wechat_redirect

# 2. Images & graphics

**Articles:**

- AndroidDeveloper官网-Guides-Images & graphics https://developer.android.com/guide/topics/graphics/
  - Handling bitmaps https://developer.android.com/topic/performance/graphics/

    主要看文末的 More resources

- AndroidDeveloper官网-Loading Large Bitmaps Efficiently https://developer.android.com/topic/performance/graphics/load-bitmap

- AndroidDeveloper官网-Caching Bitmaps https://developer.android.com/topic/performance/graphics/cache-bitmap

- AndroidDeveloper官网-Managing Bitmap Memory https://developer.android.com/topic/performance/graphics/manage-memory
- bugly-Android 开发绕不过的坑：你的 Bitmap 究竟占多大内存？ https://mp.weixin.qq.com/s?__biz=MzA3NTYzODYzMg==&mid=403263974&idx=1&sn=b0315addbc47f3c38e65d9c633a12cd6&scene=21#wechat_redirect
- bugly-舞动的表情包——浅析GIF格式图片的存储和压缩 https://mp.weixin.qq.com/s/v0pffOhjFWnVbU2lXjuEmw 或 https://blog.csdn.net/tencent_bugly/article/details/69943509

**Samples:**

- Github-[googlesamples](https://github.com/googlesamples)/android-DisplayingBitmaps  https://github.com/googlesamples/android-DisplayingBitmaps

# 3. Web
You can make your web content available to users in two ways: in a traditional web browser and in an Android application, by including a WebView in the layout. 也就是说，**加载一个网页有两种方式，要么用浏览器APP加载，要么在其他APP里使用 WebView加载.**
- WebView
   - AndroidDeveloper官网-Web-Based Content https://developer.android.com/guide/webapps/
