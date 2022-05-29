<p align="center"><img src="https://i.ibb.co/pP9FFnd/Clean.png" width="150"></a>
<h1 align="center"><b>How to uninstall Android Apps (NON-ROOT)</b></h1>
<h4 align="center">Uninstall Bloatware without Root Access (They are just being uninstalled for the current User)</h4>
<hr />
<br />

## Requirements:
* Windows OS
* Download ADBKit - [GitHub](https://github.com/K3V1991/ADBKit)
* USB Driver for your Device or Universal ADB Driver

## Enable Developer Options & USB Debugging:
1. Install the USB Driver for your Phone or Universal Adb Driver
2. On your Phone, go to Settings > About Phone. Find the Build Number and tap on it 7 times to enable Developer Options
3. Now enter System > Developer Options and find "USB debugging" and enable it
4. Plug your Phone into the Computer and change it from "Charge only" to "File Transfer" Mode
5. On your Computer, browse to the Directory where you extracted the ADBKit Zip
6. Launch a Command Prompt with Open CMD.bat
7. Once you’re in the Command Prompt, enter the following Command: 
```
adb devices
```
8. System is starting the ADB Daemon (If this is your first Time running ADB, you will see a Prompt on your Phone asking you to authorize a Connection with the Computer. Click OK.)
9. Succesful enabled USB Debugging

## Uninstall Apps: 
1. Enable adb shell, type:
```
adb shell
```
and hit Enter

2. Uninstall App (Example Package "YouTube"):
```
pm uninstall --user 0 com.google.android.youtube
```
and hit Enter
<br />

## Re-install Apps:
1. Enable adb shell, type:
```
adb shell
```
and hit Enter

2. Re-install App (Example Package "YouTube"):
```
cmd package install-existing com.google.android.youtube
```
and hit Enter
