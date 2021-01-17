---
id: googlesignin
title: Google Sign in
---

* Go back to your Firebase console
* Go to <b>Authentication -> Sign-in method</b>
* <b>Enable Google</b> and provide your support email.

![alt-text](assets/img/appconfig/googlesignin/1.png)

* Now go to the <b>Project Settings</b>

![alt-text](assets/img/appconfig/googlesignin/2.png)

* Slide down and press on <b>Add Fingerprint</b> in the Android Apps section 
* Now go back to your Android Studio and run the following command in order to get the <b>SHA1</b> and <b>SHA256</b>

```
keytool -list -v -keystore "\.android\debug.keystore" -alias androiddebugkey -storepass android -keypass android 
```

<blockquote>Note that the second command needs information from the generated signed key, if you have not generated a signed apk yet, come back later and run this second command.
</blockquote>

After running this command you will get the <b>SHA1 and SHA256</b> for development mode, we need to run the second command for the release mode. (You have to replace <b>"key"</b> with your .jks file name, and replace the path <b>"C:\Users\Gamer\key.jks"</b> to the path where your .jks is located on your machine, replace also the storepass <b>"pass"</b> and the keypass <b>"pass"</b> to your information.

```
keytool -list -v -alias key -keystore "C:\Users\Gamer\key.jks" -storepass pass -keypass pass
```

When you run the commands you get the SHA1 and the SHA256 of both the development and the release versions of your app. Copy each one and add it in your Firebase fingerprint, you will end up having 2 SHA1 keys and 2 SHA256 keys

![alt-text](assets/img/appconfig/googlesignin/3.png)

![alt-text](assets/img/appconfig/googlesignin/4.png)

* After that, you have to <b>re-download</b> <b>google-services.json</b> and <b>googleservice-info.plist</b> and replace it with your old <b>google-services.json</b> and <b>googleservice-info.plist</b> (This step is very important because the old files didn't have the SHA required for the google sign in)
