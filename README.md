## XiaomiToolV2 [Fork]

[<img alt="CI" src="https://github.com/LiohMoeller/XiaoMiToolV2/actions/workflows/ci.yml/badge.svg">](https://github.com/LiohMoeller/XiaoMiToolV2/actions/workflows/ci.yml)
[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](./LICENSE)

Source code of Xiaomi bootloader unlocking tool.

Other tools to unlock bootloader Xiaomi devices - [Awesome Xiaomi Bootloader Unlock](https://github.com/LiohMoeller/awesome-xiaomi-bootloader-unlock)

### State of the project
  - The original XiaomiToolV2 is abandoned and it needed a small correction to make it run on Linux.

### Unlock BootLoader

Sign in to your [Xiaomi account](https://account.xiaomi.com).
For this, go to Settings → Mi Account
Link your phone number to your account (It's necessary)

The first step is to enable OEM Unlocking and USB debugging on the Xiaomi phone.
For this, go to Settings → About Phone → Then Tap MIUI version 7 times to enable Developer Options.
Next go Settings → Additional settings → Developer Option.
Then Turn on the toggle button OEM Unlocking and USB debugging options.

Then Turn on your mobile data and Turn off all Wifi, Hotspot and Bluetooth.

Keep in mind, you have to turn on mobile data from the same SIM from which you have created your Mi account.

Now you have to Tap on Mi Unlock status and then tap on the Agree button.

After that, you have to tap on “Add Account and Device“.

You should receive a confirmation that the Device was added to you account.

Reboot to Fastboot.

With the device powered off, hold Volume Down + Power. Keep holding both buttons until the word “FASTBOOT” appears on the screen, then release. (For some devices there may be a different combination)

Now you can use XiaoMiToolV2 to proceed with the unlocking.

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



