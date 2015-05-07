MaterialNavigationDrawer
========================
##**Note:** This fork is for using the native translucent status bar for following the Material Design specs better.

For docs, see the original repository.

## How to use
Add this to your build.gradle:
```java 
repositories {
    maven{
        url "https://jitpack.io"
    }
}

dependencies {
    compile 'com.github.Kinnonii:MaterialNavigationDrawer:1.4.0'
}
```
If you want to use this fork, just extend the TranslucentKitKatStatusBar theme in the values-v19/styles.xml and add`<item name="android:windowTranslucentStatus">true</item>` to your styles-v21.xml. Be sure to work with dimens.xml if you have independent activities that doesn't extends from MaterialNavigationDrawer. Here are the files:

####values/dimens.xml
```xml
<dimen name="padding_app_bar_top">0dp</dimen> <!-- Apply this as paddingTop of your app_bar.xml root element -->
<dimen name="app_bar_size">56dp</dimen> <!-- Apply this as layout_height of your app_bar.xml root element -->
```
####values-v19/dimens.xml
```xml
<dimen name="padding_app_bar_top">24dp</dimen> <!-- Apply this as paddingTop of your app_bar.xml root element -->
<dimen name="app_bar_size">80dp</dimen> <!-- Apply this as layout_height of your app_bar.xml root element -->
```
####values-v21/dimens.xml
```xml
<dimen name="padding_app_bar_top">24dp</dimen> <!-- Apply this as paddingTop of your app_bar.xml root element -->
<dimen name="app_bar_size">80dp</dimen> <!-- Apply this as layout_height of your app_bar.xml root element -->
```
