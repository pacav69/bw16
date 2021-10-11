[![cavtronics logo](https://cldup.com/BhJv2ZU0rj.jpg)](http://www.cavtronics.com "cavtronics")

![<bw16 board >](<https://github.com/pacav69/bw16/blob/main/images/bw16boardfrontandback.png?raw=true>)


# Getting started 
First read document on [Getting started 
](https://www.amebaiot.com/en/amebad-bw16-arduino-getting-started/)

## Programming
The pins LOG_UART_TX (PA7) and LOG_UART_RX (PA8) are used for program upload. However, the onboard USB-to-UART module is connected to LP_UART_TX (PB1) and LP_UART_RX (PB2) and thus cannot be used directly for program upload. You can choose to either use an external USB-to-UART module connected to PA7 and PA8, or you could short these pins together to use the on-board USB for program upload:
PA8–––PB2
PA7–––PB1
After connecting accordingly, the USB driver for BW16/RTL8720DN will be automatically installed. You can check the COM port number in Device Manager of your computer:




## Layout

![< BW16 Layout>](<https://github.com/pacav69/bw16/blob/main/images/bw16layoutpinout.png?raw=true >)

## PIN Function

![<PIN Function >](<https://github.com/pacav69/bw16/blob/main/images/bw16pinfunction.png?raw=true >)