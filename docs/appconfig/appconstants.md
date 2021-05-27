---
id: appconstants
title: App Constants
---

In <b>lib/config/app_config.dart</b> there are some values that you can change

* The <b>Google Play Identifier</b> and the <b>App Store Identifier</b> are used for rating the application when it will be published.

* For Admob ads:
    * Go to https://admob.google.com/
    * Create an account
    * Go to <b>"Apps"</b> and <b>Add App</b>, you will be asked if you have published the app on Google Play or on Apple Store, for now press <b>"NO"</b>, but after that you published it you have to <b>come back</b> and <b>link your published app to the app</b> you created now in Admob.
    * Enter the App name and the platform and press <b>"ADD"</b>
    * Once done you can create a <b>Banner ad</b> and an <b>Interstitial ad</b> and place its ids in the constant file, you will also be provided with the Admob App Id replace it also in constants
    * You also have to change the <b>app id</b> in <b>"android/app/src/main/AndroidManifest.xml"</b> in  `<meta-data
            android:name="com.google.android.gms.ads.APPLICATION_ID"
            android:value="ca-app-pub-1469570455778464~1228577141" />`

<blockquote>For Admob on ios, you have to change your <b>Admob App Id</b> in <b>GADApplicationIdentifier</b> located in <b>ios/Runner/Info.plist"</b>
</blockquote>

* The last section is for the share feature of the application, change the <b>titles</b> and <b>texts</b> as you wish.

![alt-text](assets/img/appconfig/appconstants/1.png)