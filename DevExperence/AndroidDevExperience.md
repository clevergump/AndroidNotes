1. 单例的对象,在 getInstance() 时一定要做数据的reset. 否则可能会因为上次使用该对象后数据没有reset而干扰到下一次的使用.
2. 如果一个bug 出现在点击home键回到桌面以后，由于该过程同时经历了 Activity 的 onPause() 和 onStop() 的过程，所以有个较快定位问题到思路是，可以研究bug是出现在 onPause() 还是 onStop() 的阶段。


