---
id: generatesignedapk
title: Generate Signed APK / Bundle
---

### First method (using Android Studio only)

#### Step 1 
In android studio go to <b>Tools -> Flutter -> Open for Editing in Android Studio</b> as shown below, this will open the android folders separately

<blockquote>In case “Open Android module in Android Studio” option is missing, run the command <b>“flutter create .”</b> and restart Android Studio</blockquote>

![alt-text](assets/img/appconfig/generatesignedapk/1.png)

Then <b>Select New Window</b> option as shown below


![alt-text](assets/img/appconfig/generatesignedapk/2.png)

#### Step 2

Wait for while until project synchronization. After that Go to <b>Build -> GenerateSigned Bundle/APK...</b> option from menu bar as shown bellow

![alt-text](assets/img/appconfig/generatesignedapk/3.png)

#### Step 3

Select <b>Android App Bundle or APK</b> Option as per your need. (Android App Bundle is best solution) and click <b>Next</b> button.

![alt-text](assets/img/appconfig/generatesignedapk/4.png)

#### Step 4

Select <b>Create new..</b> option to generate new Signed key (When you release your app First Time)

![alt-text](assets/img/appconfig/generatesignedapk/5.png)

#### Step 5

Fill all options as follow

![alt-text](assets/img/appconfig/generatesignedapk/6.png)

<blockquote>
<b>Key store Path</b> - Path where your key store file i.e .jks file stored (as shown in the above image). <b>[Best way Select the path within your project directory.] </b>

* <b>Key store password</b> - Enter password e.g. 123456 

* <b>Key alias</b> - Enter Key alias (Name of .jks file) e.g. key 
* <b>Key Password</b> - Enter Key password (Choose different password than Key store password) e.g. key123456 
* <b>Validity(years)</b> - Keep it as it is or change as per your requirements. 
* <b>Certificate</b> - Fill certificate information (Not all fields are mandatory) Then click OK and you will get following screen...
</blockquote>

#### Step 6

![alt-text](assets/img/appconfig/generatesignedapk/7.png)

#### Step 7

Click <b>Next</b> and you will get following screen...

![alt-text](assets/img/appconfig/generatesignedapk/8.png)

Select options

<b>Build variants - release</b> and <b>Signature versions both V1 and V2</b> respectively as shown above screen shot and click <b>Finish</b> button. 

#### Step 8

Wait for a while until Gradle Build Running process complete as shown below...

![alt-text](assets/img/appconfig/generatesignedapk/9.png)

And finally you will get the <b>Generate Signed APK : (APKs) generated successfully</b> . from that click on Locate option to get Location of your <b>Generate Signed APK Key</b>. as shown bellow

![alt-text](assets/img/appconfig/generatesignedapk/10.png)

That's it you generated Signed APK successfully for your Flutter project.

<blockquote>Please DO NOT lose the key and its all information i.e. Key store path,Key store password, Key alias and Key password (Best way write down it in to the note book or make text file and store on your drive while generating it.). Without this, you won't be able to update your application because the new release will need to be signed with the same key.
</blockquote>

### Second Method (using Android Studio, Visual Studio Code or any other editors)
follow instructions in this link 
```
https://flutter.dev/docs/deployment/android​
```