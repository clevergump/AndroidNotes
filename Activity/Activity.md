# Activity Notes

## onCreate()

1. 通常都是重写 protected 的 onCreate(), 并且 super.onCreate(..) 不能省略,因为有 @CallSuper 注解定义.

   ```java
   @MainThread
   @CallSuper
   protected void onCreate(@Nullable Bundle savedInstanceState) {
   ```

2. [> Android O] 在 **>** Android O 的系统上 (即: 从Android 8.1 开始), 透明(translucent) 或浮动(floating) 的Activity 不允许设置固定方向(即: 在 Manifest 中为Activity设置属性screenOrientation 为 portrait, landscape, lock 等), 即: 只允许全屏且非透明的Activity才能设置固定方向.

   ```java
   protected void onCreate(@Nullable Bundle savedInstanceState) {
     if (getApplicationInfo().targetSdkVersion > O && mActivityInfo.isFixedOrientation()) {
       ...
         if (isTranslucentOrFloating) {
           throw new IllegalStateException(
             "Only fullscreen opaque activities can request orientation");
         }
     }
   ```

3. 在 onCreate()中, 如果 savedInstanceState != null, 会从 savedInstanceState 中恢复先前保存到该变量的一些东西.

4. 在 onCreate()中, 会分发该 Activity的 create 事件给到他所包含的  Fragment 的 FragmentManager, 借助于 FragmentController.

   ```java
   final FragmentController mFragments = FragmentController.createController(new HostCallbacks());
   protected void onCreate(@Nullable Bundle savedInstanceState) {
     ...  
     mFragments.dispatchCreate();
     ...
   }
   ```

5. 在 onCreate()中, 会去检查是否先前在 Application 中注册过 registerActivityLifecycleCallbacks 回调(可能有多个), 如果有注册, 则会调用所有这些回调接口的 onActivityCreated() 方法.

   ```java
   getApplication().dispatchActivityCreated(this, savedInstanceState);
   // Application.java:
   void dispatchActivityCreated(Activity activity, Bundle savedInstanceState) {
     Object[] callbacks = collectActivityLifecycleCallbacks(); // 回调List转换为数组
     if (callbacks != null) {
       for (int i=0; i<callbacks.length; i++) {
         ((ActivityLifecycleCallbacks)callbacks[i]).onActivityCreated(activity,
            savedInstanceState);
       }
     }
   }
   ```

6. ​