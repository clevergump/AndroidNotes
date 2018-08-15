notes for Picasso developed by square

1. 代码功能简单总结

   BitmapHunter：

   ​	进行Bitmap解码，变换等操作的具体类，例如：decode, transform

   RequestCreator：

    - 代理设置Request.Builder的一系列参数，
      - 缩放transform相关的设置: onlyScaleDown，resize, centerCrop, centerInside
      - rotate相关的设置：rotationDegrees，rotationPivotX，rotationPivotY，hasRotationPivot
      - custom transform: transform()
    - placeholder，error等的图片
    - 内存策略，网络策略