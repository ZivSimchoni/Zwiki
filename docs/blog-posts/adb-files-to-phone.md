---
title: Effortlessly transfer files to your Android device with ADB Push.
---

You can simply right click any file on your Windows Computer to send to your phone via adb push commands (without needing to type commands).

This makes file transfers significantly faster (especially when you have a large number of small files). You can also push whole folders with the click of a button just like copy and paste.

1. Download Android's SDK platform-tool from [Android developer site](https://developer.android.com/studio/releases/platform-tools). (That link is to the whole SDK - the minimal adb and fastboot version is enough)
2. Extract the content in your C drive. (or any other drive if u wish) so it'll be as following: `C:\platform-tools\<all dlls and exe files here>`
3. Copy the following code and paste it into a new .txt file on your PC.
4. *Optional steps* (skip to step 5 if you don't want to do this)
      1.  If you've extracted the files in other location - Edit the path to adb.exe file in below code.
      2.  The files will be moved to the 'Download' directory in the internal storage. **the script wont work if the folder is missing or misspelled**. You can use any folder just make sure you create the folder in your mobile and change the below code accordingly.
5. Save the file with .reg extension. (eg: adb-push.reg)
6. Double click the file to install the reg entry.
7. Enable developer options and enable usb debugging on your mobile and plug it in to your PC.
8. Accept the request for usb debugging access on your phone when you run this adb command for the first time. 
9. *Optional step* Wireless adb - first, you must use the command 'adb connect 192.168.xxx' to connect adb wirelessly first. (Replace ip address with your phones current ip address)


```{ .url .copy  title="Reg Entry"} 
    Windows Registry Editor Version 5.00

    [HKEY_CLASSES_ROOT\*\shell\ADB Push to Phone]

    [HKEY_CLASSES_ROOT\*\shell\ADB Push to Phone\command]
    @="C:\\platform-tools\\adb.exe push \"%1\" /sdcard/Download/"
    
    [HKEY_CLASSES_ROOT\Folder\shell\ADB Push to Phone]

    [HKEY_CLASSES_ROOT\Folder\shell\ADB Push to Phone\command]
    @="C:\\platform-tools\\adb.exe push \"%1\" /sdcard/Download/"
```


Personally I've used only the **wired** connection to push files and its absolutely convenient and fast.



[^1]: Inspired from [this](https://forum.xda-developers.com/t/use-adb-push-to-copy-files-to-device-at-blazing-fast-speeds-with-a-simple-right-click.4558759/) xda post