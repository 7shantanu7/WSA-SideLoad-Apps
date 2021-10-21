# WSA Installation
A simple guide to install [WSA](https://docs.microsoft.com/en-us/windows/android/wsa/) and sideload apks in WSA for non US users.

* Download WSA `.msixbundle` from [here](http://tlu.dl.delivery.mp.microsoft.com/filestreamingservice/files/433b1665-c732-486a-99ee-e2c610cd10d4?P1=1634857853&P2=404&P3=2&P4=RG1QenKx%2buGmiHbo7fvZCMGvn%2fl8XlvlAsKwH4XlZjVBn%2fUPCoh06wGs3ZJVHFZgNPRdzXvhNYw8ssj80YC%2brQ%3d%3d)
* Open Windows Terminal Admin `Win+X->Admin`
* Install `.msixbundle` using following command (change the path to the actual path):
```bash
Add-AppxPackage -Path "C:\path\to\wsa.msixbundle"
```
Done! Windows Subsytem for Android™ application should be now installed in your system.

## To sideload Apks
* Download the repository zip and extract it in your desired folder.
* Turn on developer mode on in WSA. **NOTE:**  WSA should be up and running in order to adb script to work.
* Download ADB and platform-tools from [here](https://dl.google.com/android/repository/platform-tools-latest-windows.zip) and extract it in the same directory. (`WSA-SideLoad-Apks-main/`)
* To install apps just put them in same directory and then drag and drop on `install-apk.bat`.

Done! Your Android App is now installed.
