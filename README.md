[![cavtronics logo](https://cldup.com/BhJv2ZU0rj.jpg)](http://www.cavtronics.com "cavtronics")

## BW16-RTLDuiono board
![<bw16 board >](<https://github.com/pacav69/bw16/blob/main/images/bw16boardfrontandback.png?raw=true>)

##Specifications
* 802.11 b/g/n,CMOS MAC,Baseband PHY
* CPU: Cortex-M3
* ROM: 1 MB RAM: 512 KB, FLASH: 1 MB
* WiFi @ 2.4 GHz and 5GHz，Support WPA/WPA2 Security Mode
* Support STA/AP/STA+AP Module
* SPI,UART,PWM,GPIO
* Deep Sleep Current 10 uA，Shutdown Current below 5 uA
* Use LWIP network protocol stack
* Use FreeRTOS operating system

## Setup

Open Arduino IDE. To set up AmebaD correctly in Arduino IDE, go to “File” -> “Preferences”

And paste the following URL into “Additional Boards Manager URLs” field:

	https://github.com/ambiot/ambd_arduino/raw/master/Arduino_package/package_realtek.com_amebad_index.json
	


Next, go to “Tools” -> “Board” -> “Boards Manager”:

The “Boards Manager” requires about 10~20 seconds to refresh all hardware files (if the network is in bad condition, it may take longer). Every time the new hardware is connected, we need to reopen the Board Manager. So, we close the Boards Manager, and then open it again. Find “Realtek Ameba Boards” in the list, click “Install”, then the Arduino IDE starts to download required files for AmebaD.


## Programming
### Using external programmer
The pins LOG_UART_TX (PA7) and LOG_UART_RX (PA8) are used for program upload. However, the onboard USB-to-UART module is connected to LP_UART_TX (PB1) and LP_UART_RX (PB2) and thus cannot be used directly for program upload. You can choose to either use an external USB-to-UART module connected to PA7 and PA8, 
 
### Programming through USB
Short these pins together to use the on-board USB for program upload:

* PA8–––PB2
* PA7–––PB1

After connecting accordingly, the USB driver for BW16/RTL8720DN will be automatically installed. You can check the COM port number in Device Manager of your computer:




## Layout

![< BW16 Layout>](<https://github.com/pacav69/bw16/blob/main/images/bw16layoutpinout.png?raw=true >)

## PIN Function

![<PIN Function >](<https://github.com/pacav69/bw16/blob/main/images/bw16pinfunction.png?raw=true >)