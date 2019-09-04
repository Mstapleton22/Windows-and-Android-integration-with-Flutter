## Windows and Android integration with Flutter

### Install the following:
[Android Studio](https://developer.android.com/studio/) 

[SDK Tools](https://developer.android.com/studio/releases/sdk-tools.html)

Once these two things are installed, you can go ahead and install [flutter](https://github.com/Chimer2017/xdemo_flutter) (crucial)

### Inside Android Studios follow these steps:
1. Go To...

   1. Studio
   1. File
   1. Settings 
   1. Plugins
   1. Browse Repositories
2. Search for flutter.
3. Tap on Install (a dialog will pop regarding dart dependency. click Yes).
4. Once the installation is finished restart android studio.

### For the simulator:

**If**

you have a windows machine that supports Intel processor that supports VT-x and NX,
follow [this documentation](https://developer.android.com/studio/run/managing-avds) to set up the simulator device.

**Else**

You will be prompted with the following error:

Unfortunately, your computer does not support hardware accelerated virtualization.
Here are some of your options:
 1) Use a physical device for testing (demonstration below)
 2) Develop on a Windows/OSX computer with an Intel processor that supports VT-x and NX
 3) Develop on a Linux computer that supports VT-x or SVM
 4) Use an Android Virtual Device based on an ARM system image
   (This is 10x slower than hardware accelerated virtualization)

**Option 1) Using a physical android phone:**

1. Plug in your device to your computer.

2. Using the physical android phone/tablet:
    1. Settings
    1. About phone
    1. Software information
    1. TAP “build number” 8 times.
    1. Type in pin.
    1. Developer mode will be initialized.

3. **Return to settings level** under the “about phone” folder you will see **developer options**.

4. Turn developer option **ON** and make sure **USB DEBUGGING** is **ON**.

5. In terminal **run flutter doctor**.

6. **Return to android device** click ok to **Allow USB Debugging with Computer RSA key fingerprint / access code.**
    - If you are still not seeing the fingerprint confirmation, use this [relevant article](https://www.thecustomdroid.com/enable-developer-options-usb-debugging-android-pie/) to follow the order of operations.

7. In terminal **run flutter doctor**.
   - Device should be visible from the terminal (flutter doctor) at this point.
 
8. Run **flutter run** - 
     *make sure your android device stays “Active” with a lit up screen so that the computer can use it as a simulator.
  
  
### Options 2, 3, 4)

**NOTE**
Android Studio emulator won't run on Windows with an AMD processor. The error message is kind of misleading, as it suggests the problem is with the CPU. But it is within the troubleshoot message: "Windows/OSX computer with an Intel processor".

Solutions could be installing Linux and running Android Studio on that (which might come with its own issues), using a physical device for testing or using the slow ARM images.

**Recommended**
Use an android device if it is possible.
Othewise
Download the linux machine and have fun :)
