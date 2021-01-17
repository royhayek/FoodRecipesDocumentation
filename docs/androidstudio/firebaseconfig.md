---
id: firebaseconfig
title: Firebase Configuration
---

Navigate to https://firebase.google.com/

Register or log in first and then go to console then press on <b>Create a project</b>.

![alt-text](assets/img/firebaseconfig/1.png)

In the dialog window enter the name of the project then press continue and follow instructions until the project is created.

![alt-text](assets/img/firebaseconfig/2.png)

After successfully creating a project on Firebase then the page will be redirected to the dashboard project that has been made. Then in the dashboard select Add Firebase to your Android app.

#### 1. ANDROID CONFIGURATION

![alt-text](assets/img/firebaseconfig/3.png)

In the next dialog window enter the name of the Android application package. (the package name that you will be using for your application and which will appear in the store when it is published)

![alt-text](assets/img/firebaseconfig/4.png)

Now you have to download <b>google-services.json</b> by pressing on the download button, once downloaded locate it and add it to your android studio project in <b>android -> app</b> as shown in the picture below:

![alt-text](assets/img/firebaseconfig/5.png)

#### 1. IOS CONFIGURATION (REQUIRES A MAC)

Go back to the <b>Project Overview</b> and add another app by pressing on the <b>+</b> button. Press on <b>IOS</b>

![alt-text](assets/img/firebaseconfig/6.png)

Write the package name then press on <b>Register App</b>

![alt-text](assets/img/firebaseconfig/7.png)

Download <b>GoogleService-Info.plist</b> by pressing on the download button, once downloaded go back to android studio and right click on the <b>ios</b> folder then press <b>Open in Xcode</b>. Once Xcode is open right click on the <b>Runner</b> folder and press <b>Add Files to "Runner"...</b> choose the GoogleService-Info.plist and press <b>Add</b>

As shown in the pictures below:

![alt-text](assets/img/firebaseconfig/8.png)


![alt-text](assets/img/firebaseconfig/9.png)