# android-run-debug-install-builds-over-wi-fi-macbook-pro
## android – run/debug/install builds over wi-fi macbook pro

### Connect ADB over Wi-Fi:

+ )Open a terminal on your MacBook Pro.
+ )Check if your device is connected by running:

```markdown

adb devices

```

+ )Note the device ID shown.
+ )Enable TCP/IP mode by running:
  
```markdown
adb tcpip 5555
```

+ ) Disconnect the USB cable.
+ ) Find your Android device's IP address. This can typically be found in ***Settings > About phone > Status > IP address.***
+ ) Connect to your Android device over Wi-Fi by running:
```markdown
adb connect <device_ip_address>:5555

```
Replace **<device_ip_address>** with your device's IP address.
### 3.Verify Connection:

+ ) To verify that your device is connected over Wi-Fi, run:
```markdown
adb devices

```
You should see your device listed with its IP address.

### 4.Configure Android Studio:
+ ) Open Android Studio.
+ ) Go to **Run > Edit Configurations.**
+ ) Ensure the target device is selected properly.
+ ) Start your build or debugging session as usual. Your Android device should now be accessible over Wi-Fi.


### Troubleshooting:

+ ) **Device not found:** Ensure both your MacBook Pro and Android device are on the same Wi-Fi network and there are no network restrictions.
+ ) **ADB connection lost:** Sometimes, the Wi-Fi connection might drop. Reconnect using adb connect **<device_ip_address>:5555.**
+ ) **Firewall issues:** Ensure that your network firewall is not blocking the connection on **port 5555.**


### Run android : 

**3. Reconnect the Device:**
+ ) Ensure your Android device or emulator is properly connected and recognized.
+ ) You can check connected devices by running:

```markdown

adb devices

```

### 4.Run the App:
+ ) Open another terminal, navigate to your project directory, and run:
```markdown

npx react-native run-android

```
https://chatgpt.com/c/5a61ab55-e6d7-4d90-87e7-020eb6271da3



