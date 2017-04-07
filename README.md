# PressScanCode
一个长按扫描webView上的二维码的工具库。


![](./tips.gif)

## 支持
- 任意屏幕上可见的View

## 用法

- Add it in your root build.gradle at the end of repositories:
```
	allprojects {
		repositories {
			...
			maven { url 'https://jitpack.io' }
		}
	}
  ```
  
- Add the dependency
  
  ```
  	dependencies {
	        compile 'com.github.BolexLiu:PressScanCode:v1.0.0'
	}
  ```
 - 使用
 ```
   ScanTools.scanCode(v, new ScanTools.ScanCall() {
                     @Override
                     public void getCode(String code) {
                         Toast.makeText(ScanSimpleActivity.this,code,Toast.LENGTH_SHORT).show();
                     }
                 });
 ```
