# Android-Gingerbread-Revamped
This is a small personal project of mine that makes stock Android 2.3 (Gingerbread) apps compatible with modern phones.
- Apps are tested on Android 16 HyperOS 3.0

## Apps in work:

- Alarm ⏰
- Contacts 📞
- Music 🎵
- Gallery  🖼️
- Settings ⚙️ **(May not be very compatible. If so, it will be there just for the looks)**

## Installation

**The apps still use the old SDK (8) so you will not be able to install the apps the traditional way. You're gonna have to use the ADB console to install them**
- Download [platform tools](https://developer.android.com/tools/releases/platform-tools)
- Plug in your phone with your PC
- Make sure USB Debugging on your phone is on. Here's a [guide](https://techengage.com/enable-usb-debugging-mode-on-android/) 
- Download the APK of your choice and then make a new folder on your PC which contains platform-tools and the APK.
- Open Command Prompt and use `--bypass-low-target-sdk-block` to bypass the target SDK and install the app. Just like this:
`adb install --bypass-low-target-sdk-block APP_NAME.APK`


> [!NOTE]
> Some apps (like clock) may ask for additional permissions which are not required and may seem weird for some users. That's because the target SDK is still 8 (Android 2.3) and it asks for permissions which are meant for older Android versions. I will list down below which permissions are needed for each app:

### Clock
- Show on lock screen (for the alarm)
- Open new windows while running in the background (also for the alarm)
- Access to music and audio files (For the ringtone)
