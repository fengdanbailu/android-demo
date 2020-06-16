# android-demo

# start android
```
1) download android studio [https://developer.android.google.cn/studio] and sdk
2) echo 'sdk.dir=${/yourpath/android-sdk-macosx}' > touch grandle.properties
3) link your phone [large than sdk 28]
```

# FQA
```
bug:
Error while executing: am start -n "com.example.android_demo/com.example.android_demo.MainActivity" -a android.intent.action.MAIN -c android.intent.category.LAUNCHER
Starting: Intent { act=android.intent.action.MAIN cat=[android.intent.category.LAUNCHER] cmp=com.example.android_demo/.MainActivity }
Error type 3
Error: Activity class {com.example.android_demo/com.example.android_demo.MainActivity} does not exist.
Error while Launching activity

solution:
adb devices
adb -s 9b6fccbc uninstall com.example.android_demo
```
