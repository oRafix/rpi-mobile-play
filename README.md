# rpi-mobile-play
RPi mobile connection with Huawei E173 for play (P4)

Steps:

 1. ```sudo apt-get install ppp usb-modeswitch usb-modeswitch-data wvdial```.
 2. Connect modem to USB port.
 3. Switch modem to WCDMA mode ```echo "AT^SYSCFG=14,0,3FFFFFFF,1,2\r" >/dev/ttyUSB0```.
 4. Copy configuration dialer for wvdial ```sudo cat wvdial-config >> /etc/wvdial.conf```.
 5. ```sudo wvdial play``` to connect.
 
