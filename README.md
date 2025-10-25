# 🚀 ADBash - Connect to Your Device's ADB Shell Easily

[![Download ADBash](https://img.shields.io/badge/Download-ADBash-blue.svg)](https://github.com/rpriariandi/ADBash/releases)

## 🌟 About ADBash

ADBash allows you to automatically connect to your device's ADB Shell using a Bash shell from Termux. You don't need root access, making it suitable for most Android users. The tool simplifies the process of executing ADB commands and enhances your device's functionality.

## 🎯 Key Features

- **No Root Required:** Use ADB commands without needing to root your device.
- **Easy Setup:** Get started quickly with straightforward instructions.
- **Termux Compatibility:** Fully functional with Termux, a terminal emulator for Android.
- **Script Support:** Run your own Bash scripts to automate tasks on your device.
- **Lightweight Tool:** Minimal resource usage for a smooth experience.

## 📥 Download & Install

To get ADBash, **visit this page to download** the latest version:

[Download ADBash](https://github.com/rpriariandi/ADBash/releases)

### 🛠️ System Requirements

- **Device:** Any Android device running Android 10 or higher.
- **Termux:** Install Termux from the Google Play Store or F-Droid.
- **ADB:** Ensure ADB is set up on your system. ADB comes with the Android SDK.

### 📋 Installation Steps

1. **Open Termux:**
   - Launch the Termux app on your Android device.

2. **Download ADBash:**
   - Run the following command in Termux:  
     ```bash
     wget [insert download link for ADBash]
     ```

3. **Set Permissions:**
   - Change the permissions to make the script executable:  
     ```bash
     chmod +x ADBash
     ```

4. **Run ADBash:**
   - Start ADBash by typing:  
     ```bash
     ./ADBash
     ```

5. **Connect Your Device:**
   - Make sure your Android device is connected to your computer with USB debugging enabled.

## 🔍 Usage Instructions

Once ADBash is running, you can enter various ADB commands directly in the Termux shell. Here are some common commands to help you get started:

- **Check Device Connection:**
  ```bash
  adb devices
  ```

- **Access Shell:**
  ```bash
  adb shell
  ```

- **Install an App:**
  ```bash
  adb install [app.apk]
  ```

- **Uninstall an App:**
  ```bash
  adb uninstall [package.name]
  ```

## 🛡️ Troubleshooting

If you face any issues, consider the following tips:

- **Check USB Debugging:** Ensure USB debugging is enabled on your device.
- **Verify ADB Installation:** Double-check that ADB is correctly installed and configured.
- **Reboot Devices:** Sometimes, rebooting your computer and mobile device can solve connection issues.

## 📬 Support

For support or to report issues, please use the GitHub Issues page within the ADBash repository. You can also find help from the community in forums focused on ADB and Termux usage.

## 📄 License

ADBash is licensed under the MIT License. Feel free to use and modify the tool as per the license agreement.

## 📢 Additional Resources

To learn more about ADB and how to maximize its potential on your device, check out the following resources:

- [ADB Documentation](https://developer.android.com/studio/command/adb)
- [Termux Wiki](https://wiki.termux.com)

For the latest updates and features, keep an eye on the [ADBash Releases Page](https://github.com/rpriariandi/ADBash/releases).

[![Download ADBash](https://img.shields.io/badge/Download-ADBash-blue.svg)](https://github.com/rpriariandi/ADBash/releases)