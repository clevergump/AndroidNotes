# 0. Android 工具
- dumpsys   
   - AndroidDeveloper官网 https://developer.android.com/studio/command-line/dumpsys   

# 1. performance
## (0) General
- fish-Android性能检测工具 https://zhuanlan.zhihu.com/p/31828854

## (1) ANR
- gityuan-Input系统—ANR原理分析(原理) http://gityuan.com/2017/01/01/input-anr/
- duanqz-ANR机制以及问题分析(原理+实战) http://duanqz.github.io/2015-10-12-ANR-Analysis

## (2) RAM
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
   - MAT - Memory Analyzer Tool 使用进阶 http://www.lightskystreet.com/2015/09/01/mat_usage/
   - bugly-Android 开发绕不过的坑：你的 Bitmap 究竟占多大内存？ https://mp.weixin.qq.com/s?__biz=MzA3NTYzODYzMg==&mid=403263974&idx=1&sn=b0315addbc47f3c38e65d9c633a12cd6&scene=21#wechat_redirect
- 原理
   - LeakCanary:
      - LeakCanary 内存泄露监测原理研究 https://www.jianshu.com/p/5ee6b471970e
      - fish-LeakCanary原理解析 https://zhuanlan.zhihu.com/p/34672399
- 实例
   - wetest-LeakCanary+Jenkins内存泄漏监控实践 http://wetest.qq.com/lab/view/175.html
   - wetest-专项：Android 内存泄露实践分析 http://wetest.qq.com/lab/view/161.html


# 2. Images & graphics

**Articles:**

- AndroidDeveloper官网-Guides-Images & graphics https://developer.android.com/guide/topics/graphics/
  - Handling bitmaps https://developer.android.com/topic/performance/graphics/

    主要看文末的 More resources

- AndroidDeveloper官网-Loading Large Bitmaps Efficiently https://developer.android.com/topic/performance/graphics/load-bitmap

- AndroidDeveloper官网-Caching Bitmaps https://developer.android.com/topic/performance/graphics/cache-bitmap

- AndroidDeveloper官网-Managing Bitmap Memory https://developer.android.com/topic/performance/graphics/manage-memory
- bugly-Android 开发绕不过的坑：你的 Bitmap 究竟占多大内存？ https://mp.weixin.qq.com/s?__biz=MzA3NTYzODYzMg==&mid=403263974&idx=1&sn=b0315addbc47f3c38e65d9c633a12cd6&scene=21#wechat_redirect

**Samples:**

- Github-[googlesamples](https://github.com/googlesamples)/android-DisplayingBitmaps  https://github.com/googlesamples/android-DisplayingBitmaps

