---
id: appicon
title: App Icon
---

To change your app icon follow the steps below:

#### Step 1 
Add your logo in <b>"assets/images"</b>

![alt-text](assets/img/appicon/1.png)

#### Step 2
Open <b>pubspec.yaml</b> and change the edit the image_path in this way <b>"assets/images/your_icon_name.png"</b> (or jpg depending on your icon)

![alt-text](assets/img/appicon/2.png)

#### Step 3
Open the Terminal from the bottom of the screen

![alt-text](assets/img/appicon/3.png)

And execute the below commands in the terminal 

```
flutter pub get
```
```
flutter pub pub run flutter_launcher_icons:main
```

After that, your icon will be updated