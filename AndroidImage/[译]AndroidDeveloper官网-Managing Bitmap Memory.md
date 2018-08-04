[翻译]AndroidDeveloper官网-Managing Bitmap Memory 

原文地址：https://developer.android.com/topic/performance/graphics/manage-memory

# Android Bitmap 内存管理的演进史

1. GC

   | Android 版本      | GC类型                | 说明                                  |
   | --------------- | ------------------- | ----------------------------------- |
   | \<= Android 2.2 | 串行GC                | 当GC发生时，整个线程会停止                      |
   | \>= Android 2.3 | 并行GC(concurrent GC) | 当一个Bitmap对象不再被引用而被GC回收时，系统会立即重新申请内存 |

2. 占用的内存类型

   | Android版本        | Bitmap对象本身占用的内存 | Bitmap对象中存储的像素数据占用的内存 |
   | ---------------- | --------------- | --------------------- |
   | <= Android 2.3.3 | Dalvik heap     | **native heap**       |
   | Andoird 3.0~7.1  | Dalvik heap     | Dalvik heap           |
   | >= Android 8.0   | Dalvik heap     | **native heap**       |

## Android 3.0 及以上系统的Bitmap内存管理

BitmapFactory.Options.inBitmap