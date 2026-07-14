# 小克浏览器

## 打包步骤

1. 下载安装 Android Studio（免费）
   https://developer.android.com/studio

2. 打开 Android Studio → File → Open → 选这个文件夹

3. 等待 Gradle 同步完成（需要联网，第一次比较慢）

4. Build → Build Bundle(s) / APK(s) → Build APK(s)

5. APK 在 `app/build/outputs/apk/debug/app-debug.apk`
   传到手机安装就好了

## 功能

- 网页全屏显示，保留状态栏
- 前进、后退、刷新、回主页
- 支持相机、麦克风、定位、文件上传
- 默认主页是 claude.ai
- 支持从其他 app 跳转打开链接
- 地址栏输入网址或关键词（自动搜索）

## 改主页

MainActivity.java 最后一行改 URL 就行：
loadUrl("https://你想要的网址");
