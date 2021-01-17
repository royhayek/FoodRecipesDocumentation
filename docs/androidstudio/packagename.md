---
id: packagename
title: Package Name
---

#### ANDROID PACKAGE NAME:
##### Step 1 

1. Open <b>Gradle Scripts → build.gradle (Module: app)</b>

![alt-text](assets/img/packagename/1.png)

2. Change the application ID with your own id name
3. Standard naming procedure: <b>com.yourdomainname.yourappname</b>
4. Change the id, make it as unique as possible, because application id is very important if you want to publish the application in the store.

<blockquote><b>Important:</b> your applicationId or package name must be the same to the package name you’ve create in your firebase console when generating google-services.json</blockquote>

##### Step 2 
1. Click once on your package and then press on the settings icon at the top next to "Project". 
2. Unselect Compact Middle Packages 
3. Right click on "com", "example", and "foodrecipes" folders and rename it to your package name. 
(replace "example" by your domain name and "foodrecipes" by your app name)

![alt-text](assets/img/packagename/2.png)

![alt-text](assets/img/packagename/3.png)

#### IOS PACKAGE NAME:

In iOS, the package name is found in <b>"Runner.xcodeproj/project.pbxproj"</b>:
```
PRODUCT_BUNDLE_IDENTIFIER = com.example.appname;
```
But there are 3 lines of <b>PRODUCT_BUNDLE_IDENTIFIER</b> in <b>"project.pbxproj"</b> which you have to edit, locate it by pressing <b>CTRL + F</b> and look for <b>PRODUCT_BUNDLE_IDENTIFIER</b>. 

##### Last Step 
In order for the rate option to work in the application you have to update your Google Play and your App Store identifiers. To do that go to <b>"lib/constants.dart"</b> and change the <b>GooglePlayIdentifier</b> value to your package name and the <b>AppStoreIdentifier</b> value to your App store identifier.