## **Simple Updater For Your App!**

**How to Use**
**Step 1.** Add the JitPack repository to your build file
```css
allprojects {
		repositories {
			...
			maven { url 'https://jitpack.io' }
		}
	}
```
**Step 2.** Add the dependency
```css
dependencies {
	        implementation 'com.github.KhunHtetzNaing:AppUpdater:1.0'
	}
```
[![](https://jitpack.io/v/KhunHtetzNaing/AppUpdater.svg)](https://jitpack.io/#KhunHtetzNaing/AppUpdater)

***Example Code:***

    @Override  
    protected void onCreate(Bundle savedInstanceState) {  
        super.onCreate(savedInstanceState);  
      setContentView(R.layout.activity_main);  
      String check_update_json = "https://myappupdateserver.blogspot.com/2019/06/zfont.html";  
      AppUpdater appUpdater = new AppUpdater(this, check_update_json);  
      appUpdater.check();  
    }

## ***check_update_json* example**

Yo**u can use own server url or blogspot url!**

    {
      "title": "This is Title!",
      "message": "This is Message",
      "download": "Direct APK Download Link!!!",
      "playstore": "com.mgngoe.zfont",
      "uninstall": false,
      "what": {
        "model": [],
        "version": [],
        "all": true
      },
      "versionName": "1.7",
      "versionCode": 8,
      "force": true
    }
**Enjoy ;)**