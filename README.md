atmega16u2-adc
==============
- https://github.com/dirkarnez/ringbuffer
- https://github.com/dirkarnez/lufa-playground

### Datasheet
- https://ww1.microchip.com/downloads/en/DeviceDoc/doc7799.pdf

### Notes
- `"%LOCALAPPDATA%\Arduino15\packages\arduino\tools\avrdude\6.3.0-arduino17/bin/avrdude" "-C%LOCALAPPDATA%\Arduino15\packages\arduino\tools\avrdude\6.3.0-arduino17/etc/avrdude.conf" -v -p m16u2 -c arduino -PCOM5 -b19200 -U flash:w:Keyboard.hex:i -F -D`
- datasheet
  - `PDO, SPI Serial Programming Data Output. During Serial Program Downloading, this pin is used as data output line for the AT90USB82/162. `

### Bootloader
- [Pro Micro & Fio V3 Hookup Guide - SparkFun Learn](https://learn.sparkfun.com/tutorials/pro-micro--fio-v3-hookup-guide/troubleshooting-and-faq)
- [Installing an Arduino Bootloader - SparkFun Learn](https://learn.sparkfun.com/tutorials/installing-an-arduino-bootloader)
### Reference
- [Arduino入門教學(17) – 如何用 Arduino 燒錄 AVR 晶片 (作者：Cooper Maa)](http://programmermagazine.github.io/201405/htm/article1.html)
- [**Arduino 烧录 Boot Loader | 米米的博客**](https://zhangshuqiao.org/2019-10/Arduino%E7%83%A7%E5%BD%95Boot%20Loader/)
- [analogRead() - Arduino Reference](https://www.arduino.cc/reference/en/language/functions/analog-io/analogread/)
- https://github.com/arduino/ArduinoCore-avr/blob/master/firmwares/atmegaxxu2/arduino-usbserial/Arduino-usbserial-atmega16u2-Uno-Rev3.hex
  - `avrdude -p at90usb82 -F -P usb -c avrispmkii -U flash:w:UNO-dfu_and_usbserial_combined.hex -U lfuse:w:0xFF:m -U hfuse:w:0xD9:m -U efuse:w:0xF4:m -U lock:w:0x0F:m`
- https://github.com/arduino/ArduinoCore-avr/tree/master/firmwares/arduinoISP
  - https://github.com/arduino/ArduinoCore-avr/tree/master/firmwares/atmegaxxu2
- [用 AVR 做 USB 應用的考察 | Kalan's Blog](https://blog.kalan.dev/posts/2021-11-24-avr-usb-capability)
- [Arduino ATmega16U2 编译 LUFA_arduino mega16u2 源码-CSDN博客](https://blog.csdn.net/wowocpp/article/details/80626065)
