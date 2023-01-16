# D6 Fitness Tracker Arduino Core for Nordic Semiconductor nRF5 based boards

This core is edited for the D6 Fitness Tracker, it is original from here https://github.com/atc1441/D6-arduino-nRF5, which has much of the documentation.



## Installing

### Board Manager

 1. [Download and install the Arduino IDE](https://www.arduino.cc/en/Main/Software) (At least v1.6.12)
 2. Start the Arduino IDE
 3. Go into Preferences
 4. Add ```https://ljunquera.github.io/package_smartwatch-boards_index.json``` as an "Additional Board Manager URL"
 5. Open the Boards Manager from the Tools -> Board menu and install "D6 Tracker by ATC1441"
 6. Select the DSD6 Tracker board from the Tools -> Board menu
 7. You will find the DFU update file in a folder like this on windows. ```C:\Users\USERNAME\AppData\Local\Temp\arduino_build_RANDOM\SKETCHNAME.ino.zip```


## JSON File
---
{
    "packages": [
        {
            "name": "smartwatch-boards",
            "maintainer": "ljunquera, editied from ATC1441, edited from sandeepmistry",
            "websiteURL": "https://github.com/ljunquera/arduino-smartwatch-boards",
            "email": "D6Fitness@43u.de",
            "help": {
                "online": "https://github.com/ljunquera/arduino-smartwatch-boards/issues"
            },
            "platforms": [
                {
                    "name": "Smartwatch Boards",
                    "architecture": "nRF5",
                    "version": "0.1.2",
                    "category": "Contributed",
                    "help": {
                        "online": "https://github.com/atc1441/D6-arduino-nRF5/issues"
                    },
                    "url": "https://github.com/ljunquera/arduino-smartwatch-boards/archive/refs/tags/0.1.2.tar.gz",
                    "archiveFileName": "arduino-smartwatch-boards-0.1.2.tar.gz",
                    "checksum": "MD5:237bf3a8bc56b51bd6c8e9c95ee3732e",
                    "size": "15600126",
                    "boards": [
                        {
                            "name": "Kalinco p22"
                        },
                        {
                            "name": "DaFit Watch Bootloader 23"
                        }
                    ],
                    "toolsDependencies": [
                        {
                        "packager": "nRF52D6Fitness",
                        "name": "gcc-arm-none-eabi",
                        "version": "5_2-2015q4"
                        },
                        {
                        "packager": "nRF52D6Fitness",
                        "name": "openocd",
                        "version": "0.10.0-dev.nrf5"
                        }
                    ]
                }
            ],
            "tools": [
                {
                    "name": "gcc-arm-none-eabi",
                    "version": "5_2-2015q4",
                    "systems": [
                        {
                            "host": "i386-apple-darwin11",
                            "url": "https://github.com/sandeepmistry/arduino-nRF5/releases/download/tools/gcc-arm-none-eabi-5_2-2015q4-20151219-mac.tar.bz2",
                            "archiveFileName": "gcc-arm-none-eabi-5_2-2015q4-20151219-mac.tar.bz2",
                            "size": "96372129",
                            "checksum": "MD5:603bcce8e59683ac27054b3197a53254"
                        },
                        {
                            "host": "i686-linux-gnu",
                            "url": "https://github.com/sandeepmistry/arduino-nRF5/releases/download/tools/gcc-arm-none-eabi-5_2-2015q4-20151219-linux.tar.bz2",
                            "archiveFileName": "gcc-arm-none-eabi-5_2-2015q4-20151219-linux.tar.bz2",
                            "size": "92811866",
                            "checksum": "MD5:f88caac80b4444a17344f57ccb760b90"
                        },
                        {
                            "host": "x86_64-pc-linux-gnu",
                            "url": "https://github.com/sandeepmistry/arduino-nRF5/releases/download/tools/gcc-arm-none-eabi-5_2-2015q4-20151219-linux.tar.bz2",
                            "archiveFileName": "gcc-arm-none-eabi-5_2-2015q4-20151219-linux.tar.bz2",
                            "size": "92811866",
                            "checksum": "MD5:f88caac80b4444a17344f57ccb760b90"
                        },
                        {
                            "host": "i686-mingw32",
                            "url": "https://github.com/sandeepmistry/arduino-nRF5/releases/download/tools/gcc-arm-none-eabi-5_2-2015q4-20151219-win32.tar.bz2",
                            "archiveFileName": "gcc-arm-none-eabi-5_2-2015q4-20151219-win32.tar.bz2",
                            "size": "102981732",
                            "checksum": "MD5:32d950225b6c7c886f6225c1fc578934"
                        }
                    ]
                },
                {
                    "name": "openocd",
                    "version": "0.10.0-dev.nrf5",
                    "systems": [
                        {
                            "host": "i386-apple-darwin11",
                            "url": "https://github.com/sandeepmistry/arduino-nRF5/releases/download/tools/openocd-osx-0.10.0-dev-nrf5.tar.gz",
                            "archiveFileName": "openocd-osx-0.10.0-dev-nrf5.tar.gz",
                            "size": "1345243",
                            "checksum": "MD5:3ffaa4e7cd4b96770eec65002c5959e3"
                        },
                        {
                            "host": "i686-linux-gnu",
                            "url": "https://github.com/sandeepmistry/arduino-nRF5/releases/download/tools/openocd-linux32-0.10.0-dev-nrf5.tar.gz",
                            "archiveFileName": "openocd-linux32-0.10.0-dev-nrf5.tar.gz",
                            "size": "3585042",
                            "checksum": "MD5:02b3f4a3004cae86631bf13837c84504"
                        },
                        {
                            "host": "x86_64-pc-linux-gnu",
                            "url": "https://github.com/sandeepmistry/arduino-nRF5/releases/download/tools/openocd-linux32-0.10.0-dev-nrf5.tar.gz",
                            "archiveFileName": "openocd-linux32-0.10.0-dev-nrf5.tar.gz",
                            "size": "3585042",
                            "checksum": "MD5:02b3f4a3004cae86631bf13837c84504"
                        },
                        {
                            "host": "i686-mingw32",
                            "url": "https://github.com/sandeepmistry/arduino-nRF5/releases/download/tools/openocd-win32-0.10.0-dev-nrf5.tar.gz",
                            "archiveFileName": "openocd-win32-0.10.0-dev-nrf5.tar.gz",
                            "size": "5498373",
                            "checksum": "MD5:3acd3b08afda2bb09e75a0de5ac7c3cd"
                        }
                    ]
                }
            ]
            }
    ]
}
---
