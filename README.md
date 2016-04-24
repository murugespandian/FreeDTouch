# FreeDTouch
3D Touch API for Android

# How do I use it?
```java
FreeDTouch.OnFreeDTouchListener freeDTouchListener = new FreeDTouch.OnFreeDTouchListener() {
    @Override
    public void onFreeDTouch() {
        Toast.makeText(getApplicationContext(), "onFreeDTouch", Toast.LENGTH_SHORT).show();
    }

    @Override
    public void onLeave() {
        Toast.makeText(getApplicationContext(), "onLeave", Toast.LENGTH_SHORT).show();
    }
};

...

FreeDTouch.setup(view, freeDTouchListener)
    .setVibration(boolean)         // Default: true
    .setVibrationDuration(int)     // Default: 100ms
    .setRecyclerView(RecyclerView) // Add support for RecyclerView
    .start(); 
```
