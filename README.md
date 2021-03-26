ESP32 Bluetooth A2DP-SOURCE using I2S external source
========================
This demo is based on ESP-IDF A2DP-SOURCE code. The demo is modified so bluetooth sink (speaker) is sourced with audio via I2S external source at 48000 sample rate. The standard demo's connect/disconnect looping mode is disabled. You can specify a BT MAC to skip pairing/discovery mode using UART2. 

### Hardware Required

This example is able to run on any commonly available ESP32 development board. The I2S input should be connected to I2S ESP32 pins. 
I2S pinout:
- I2S_PIN_BCK - D26
- I2S_PIN_LRCK - D25
- I2S_PIN_BCK - D27

MGMT UART pinout:
- UART Tx - D4
- UART Rx - D5

### BT Security Database
To delete ALL existing BT paired devices, push RESET button and then immediately hold down BOOT button (do not hold down BOOT while pressing RESET! that would place the device in download mode.)

