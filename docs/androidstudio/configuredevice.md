---
id: configuredevice
title: Configure Device
---

To prepare to run and test your Flutter app on an Android device, you’ll need an Android device running Android 4.1 (API level 16) or higher.

1. Enable <b>Developer options</b> and <b>USB debugging</b> on your device. Detailed instructions are
available in the Android documentation.

2. Windows-only: Install the <b>Google USB Driver</b>.

3. Using a USB cable, plug your phone into your computer. If prompted on your device,
<b>authorize</b> your computer to access your device.

4. In the terminal, run the flutter devices command to verify that Flutter recognizes your
connected Android device. By default, Flutter uses the version of the Android SDK
where your adb tool is based. If you want Flutter to use a different installation of the
Android SDK, you must set the ANDROID_HOME environment variable to that
installation directory.

<blockquote><b>Note:</b> Sometimes you have to specify the project SDK manually in order for your device to be detected in Android Studio you can do it by going to "File" -> "Project Structure" and in the "Project SDK" press on Android API Platform.</blockquote>