← [Back to Menu](https://telinkgithub.github.io/Telink/ "Menu")
![header-telink](https://i.imgur.com/5kRG6CF.jpg)

# 826x BLE RCU Quick Start

## Features

The RC demo supports the following features:

* Works with dual batteries
* 25 valid buttons and 1 indicating LED
* Telink proprietary voice service
* Voice compressed with ADPCM, supported sample rate 16khz/16bit
* OTA firmware upgrade
* PC tool for button display and demonstration
* Low power consumption

This quick start guide uses the Telink 8267 RCU demo as an step-by-step example to show how to get the RCU sample up and running quickly. For other flavors of RCU, the steps may differ slightly, please refer to the corresponding user guide.


### Setup Guide on BLE Remote Control

__Step 1__: The appearance of the 8267RCU and dongle are as follows:

![8257RCU-dongle-appearance-1](https://telinkgithub.github.io/Assets/15_826x-BLE-RCU-Quick-Start/8267rcu.png)
![8257RCU-dongle-appearance-2](https://telinkgithub.github.io/Assets/15_826x-BLE-RCU-Quick-Start/20181022-152642.png)


__Step 2__: Download the remote.bin file to the RCU ([Burning and Debugging Tool](https://telinkgithub.github.io/Programming-and-Debugging/))

This is the RCU bin link: [8267_remote.bin](https://telinkgithub.github.io/Assets/15_826x-BLE-RCU-Quick-Start/remote_bin.zip)

This is the dongle bin link: [8266_master_kma_dongle.bin](https://telinkgithub.github.io/Assets/15_826x-BLE-RCU-Quick-Start/master_kma_dongle_bin.zip)

8267 Remote Control bin file is generated under “ble_sdk_lt_app” SDK using “826x_ble_remote” project and “8267_ble_remote” compile option as shown below.

![Step 2](https://telinkgithub.github.io/Assets/15_826x-BLE-RCU-Quick-Start/8267rcucompile.png)


__Step 3__: Connect and pair method

Power on the RCU, and RCU will be advertise state for 60 seconds.

Plug dongle into PC, then press the SW1 and that will trigger dongle to receive advertise packets. When dongle red led is on, it indicates RCU connect to dongle.


__Step 4__: BLE button and voice test method

We can just open Notepad on PC side, and when you press the number key, the number will be display in the txt file.That is button's operation.

When need to use the voice function, you can open the PC software audacity. click the record icon to start recording. Then press and hold the MIC key ![MIC key](https://telinkgithub.github.io/Assets/15_826x-BLE-RCU-Quick-Start/voicebutton.png) over 1 second,and you will see that the audacity starts to record voice data.


← [View the Project on GitHub](https://github.com/TelinkGithub/826x-BLE-RCU-Quick-Start)


![footer-telink](https://telinkgithub.github.io/Assets/General/footer.jpg)



