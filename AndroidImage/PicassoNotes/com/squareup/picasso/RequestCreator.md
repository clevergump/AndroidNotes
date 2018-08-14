# RequestCreator.java

1. public void into(ImageView target, Callback callback)

   ```
   <em>Note:</em> The {@link Callback} param is a strong reference and will prevent your
   {@link android.app.Activity} or {@link android.app.Fragment} from being garbage collected. If you use this method, it is <b>strongly</b> recommended you invoke an adjacent {@link Picasso#cancelRequest(android.widget.ImageView)} call to prevent temporary leaking.
   ```

