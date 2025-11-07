## XiaomiToolV2 [Fork]

[<img alt="CI" src="https://github.com/LiohMoeller/XiaoMiToolV2/actions/workflows/ci.yml/badge.svg">](https://github.com/LiohMoeller/XiaoMiToolV2/actions/workflows/ci.yml)
[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](./LICENSE)

Source code of Xiaomi bootloader unlocking tool.

Other tools to unlock bootloader Xiaomi devices - [Awesome Xiaomi Bootloader Unlock](https://github.com/LiohMoeller/awesome-xiaomi-bootloader-unlock)

### State of the project
  - The original XiaomiToolV2 is abandoned and it needed a small correction to make it run on Linux.

### Xiaomi Bootloader Unlock - Step-by-Step

1. **Sign in to your Xiaomi account.**  
   Go to `Settings → Mi Account`  
   Link your phone number to your account *(required)*

2. **Enable OEM Unlocking and USB Debugging:**  
   - Go to `Settings → About Phone`  
   - Tap **MIUI version** 7 times to enable Developer Options  
   - Go to `Settings → Additional settings → Developer Options`  
   - Turn ON the toggle for **OEM Unlocking** and **USB debugging**

3. **Prepare your device connection:**  
   - Turn ON mobile data, and turn OFF Wi-Fi, Hotspot, and Bluetooth  
   - Use mobile data from the SAME SIM used when creating your Mi account

4. **Add Device to Unlock Status:**  
   - Tap **Mi Unlock status**  
   - Tap **Agree**  
   - Tap **Add Account and Device**  
   - Ensure your SIM has sufficient balance to avoid warnings  
   - You should receive confirmation that your device was added successfully

5. **Reboot to Fastboot mode:**  
   - Power OFF the device  
   - Hold **Volume Down + Power** until the word *FASTBOOT* appears, then release  
   *(Note: Some devices may use a different key combination)*

6. **Proceed with unlocking:**  
   - Now you can use XiaoMiToolV2 to proceed with the unlocking.

### Building and Running

1. Install Java 21:

#### Ubuntu
```sh
sudo apt install openjdk-21-jdk git
```

#### Fedora
```sh
sudo dnf install java-21-openjdk-devel git
```

2. Download this repo:
```sh
git clone https://github.com/LiohMoeller/XiaoMiToolV2.git && cd XiaoMiToolV2
```
or
```sh
wget https://github.com/LiohMoeller/XiaoMiToolV2/archive/refs/heads/main.zip && cd XiaoMiToolV2
```

3. Build:
```sh
./gradlew build
```

4. Run:
```sh
chmod +x ./res/tools/lin/adb
chmod +x ./res/tools/lin/fastboot
./gradlew run
```

## Credits

[XiaoMiToolV2 Original](https://github.com/francescotescari/XiaoMiToolV2)

[XiaoMiToolV2 Fork 1](https://github.com/Nik-Kot/XiaoMiToolV2/tree/linux)

[XiaoMiToolV2 Fork 2](https://github.com/tkapias/XiaoMiToolV2)

[XiaoMiToolV2 Fork 3](https://github.com/topminipie/XiaoMiToolV2)

[XiaoMiToolV2 Fork 4](https://github.com/xchacha20-poly1305/XiaoMiToolV2)

[Pull Request 1](https://github.com/francescotescari/XiaoMiToolV2/pull/103)

[Pull Request 2](https://github.com/francescotescari/XiaoMiToolV2/pull/98)




