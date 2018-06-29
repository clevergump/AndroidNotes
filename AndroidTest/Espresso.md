# Espresso

包名: android.support.test.espresso

**Espresso 常用的API:**

1. Espresso.在哪个View上.执行什么动作

   ```java
   // onView(..)不能用于AdapterView, 如需匹配AdapterView,请使用 Espresso.onData(..)
   Espresso.onView(ViewMatchers....).perform(ViewActions...); // 非AdatperView
   Espresso.onData(..).perform(ViewActions...); // AdatperView
   ```

2. Espresso.在哪个View上.验证什么结果

   ```java
   // onView(..)不能用于AdapterView, 如需匹配AdapterView,请使用 Espresso.onData(..)
   Espresso.onView(ViewMatchers....).check(ViewAssertions...); // 非AdatperView
   Espresso.onData(..).check(ViewAssertions...); // AdatperView
   ```

**常用的工具类:**

Espresso, ViewMatchers, ViewActions, ViewAssertions

| Espresso常用工具类 | 用途                                       | 常用方法举例                                   | 关联类或接口                                   |
| ------------- | ---------------------------------------- | ---------------------------------------- | ---------------------------------------- |
| Espresso      | Espresso框架的入口类                           | onView(Matcher<View>), onData(Matcher<? extends Object> |                                          |
| ViewMatchers  | 获取匹配器对象的工具类,需要设定与特定View进行匹配的条件, 例如:可以设置匹配View在布局文件中定义的 id | withId(int)                              | org.hamcrest.Matcher                     |
| ViewActions   |                                          |                                          | android.support.test.espresso.ViewAction |



