---
id: facebooksignin
title: Facebook Sign in
---


* Go back to your Firebase console 
* And press on <b>Add iOS app</b>
* Provide the app name and press <b>Register App</b>
* Then download the <b>GoogleService-info.plist</b> and place it in <b>"ios/Runner"</b>
* Open <b>GoogleService-info.plist</b> and look for ```<key>REVERSED_CLIENT_ID</key>```
* Copy its <b>string value</b> (e.g. com.googleusercontent.apps.397983933757-o1dpcdnom2bhnnalk67pctjp4rkpvfba) 

![alt-text](assets/img/appconfig/facebooksignin/1.png)

* And paste it in <b>Info.plist</b>

![alt-text](assets/img/appconfig/facebooksignin/2.png)

* Now go to https://developers.facebook.com/docs/facebook-login/ios and create a new app.

![alt-text](assets/img/appconfig/facebooksignin/3.png)

* After creating the app, slide down, enter your app <b>Bundle ID</b> (package name), and <b>save</b>.

![alt-text](assets/img/appconfig/facebooksignin/4.png)

* Now go to <b>My apps</b> from the top navigation bar and go to your created app. in the left panel you will <b>Facebook Login</b>, press on <b>quickstart</b> and select <b>android</b>, keep pressing next until you reach step 3 then write your <b>package name</b> and your </b>package name.MainActivity</b> and save.
* Go to the next step. Here we have <b>2 commands</b> that we have to run in order to get <b>Key Hashes</b>.
* First of all, run the first windows command in your windows <b/>command prompt</b> (if you are using mac use the mac terminal) 
* And add the <b>Key hash</b> that you get from the command in the <b>Facebook login quickstart</b> as shown in the image below.

<blockquote>If you don't have openssl in your machine, download it from google and extract it to your C or D drive then go to <b>Environmental Settings</b> and add the openssl folder path (e.g. C:\Users\Gamer\openssl\bin)to <b>"PATH"</b> in the user variables. then run the command</blockquote>

![alt-text](assets/img/appconfig/facebooksignin/5.png)

* Now run the second command, (which is the release command, do this step after generating the signed apk, same thing as running the keytool command for release) by replacing the alias <b>"YOUR_RELEASE_KEY_ALIAS"</b> to your previously named <b>key</b> (it was previously named "key" when we were generating the SHA1 and SHA256 keys) and replace the <b>"YOUR_RELEASE_KEY_PATH"</b> to your <b>.jks key file path</b>.

* Add also the <b>Key hash</b> that you get from the command in the <b>Facebook login quickstart</b>.

<blockquote> Later on if you get an error saying that a specific Key Hash is not found or not set when running the app and sign in using facebook, write that Key Hash also in the Facebook Login Quickstart.
</blockquote>


* Now keep pressing Next till the end
* To finish the Facebook connection locate your App ID copy and paste it in your Info.plist

![alt-text](assets/img/appconfig/facebooksignin/6.png)

![alt-text](assets/img/appconfig/facebooksignin/9.png)

<blockquote>Keep the <b>"fb"</b> word before the <b>App ID</b> in the <b>CFBundleURLSchemes</b>, do not remove it</blockquote>

* The same thing for android, go to <b>android -> app -> src -> main -> res -> values</b> and open <b>strings.xml</b> then replace your <b>Facebook App ID</b> there in the 2 places.

![alt-text](assets/img/appconfig/facebooksignin/7.png)

* The last step has to be done after publishing the application on the store, go back to your facebook developer console and turn on the "In development" switch, you will be asked to enter your privacy policy url, you should create one and provide the url, you may host it with the admin panel files ( it will also be used in your application by replacing it in your admin panel settings and it will be displayed in the application for users). They may also ask you to provide a privacy policy in the Google Play Console.

![alt-text](assets/img/appconfig/facebooksignin/8.png)









