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


### ./gradle clean 

**Ý nghĩa:** <br>
Lệnh này được sử dụng để xóa thư mục **build** trong dự án của bạn. Thư mục **build** chứa các file tạm thời và các kết quả biên dịch trước đó. Khi bạn chạy lệnh **clean, Gradle** sẽ xóa tất cả các file này để đảm bảo rằng lần xây dựng **(build)** tiếp theo sẽ diễn ra từ đầu **(fresh build).** <br><br>

```sh
./gradlew clean

```


###  ./gradle --stop:
**Ý nghĩa:** <br>
Lệnh này được sử dụng để dừng tất cả các daemon Gradle đang chạy. Gradle daemon là một tiến trình chạy ngầm nhằm tăng tốc độ xây dựng dự án. Tuy nhiên, đôi khi bạn cần dừng các daemon này, chẳng hạn như khi bạn muốn giải phóng bộ nhớ hoặc khi gặp vấn đề với daemon hiện tại. <br><br>

```sh
./gradlew --stop

```


### IDE android studio : 

![Screenshot 2024-07-31 at 13 26 43](https://github.com/user-attachments/assets/3a8fe290-4794-4079-86c2-a88daa14fdc2) <br><br>
![Screenshot 2024-07-31 at 13 29 16](https://github.com/user-attachments/assets/a41bafad-e56e-4cf1-9acb-2f6ab3b9a276) <br><br>




