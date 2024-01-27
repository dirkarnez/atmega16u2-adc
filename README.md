atmega16u2-adc
==============
- https://github.com/dirkarnez/ringbuffer
- https://github.com/dirkarnez/lufa-playground

### Datasheet
- https://ww1.microchip.com/downloads/en/DeviceDoc/doc7799.pdf

### Notes
- `"%LOCALAPPDATA%\Arduino15\packages\arduino\tools\avrdude\6.3.0-arduino17/bin/avrdude" "-C%LOCALAPPDATA%\Arduino15\packages\arduino\tools\avrdude\6.3.0-arduino17/etc/avrdude.conf" -v -p m16u2 -c arduino -PCOM5 -b19200 -U flash:w:Keyboard.hex:i -F -D`


### Reference
- [Arduino入門教學(17) – 如何用 Arduino 燒錄 AVR 晶片 (作者：Cooper Maa)](http://programmermagazine.github.io/201405/htm/article1.html)
- [**Arduino 烧录 Boot Loader | 米米的博客**](https://zhangshuqiao.org/2019-10/Arduino%E7%83%A7%E5%BD%95Boot%20Loader/)
- [analogRead() - Arduino Reference](https://www.arduino.cc/reference/en/language/functions/analog-io/analogread/)
- https://github.com/arduino/ArduinoCore-avr/blob/master/firmwares/atmegaxxu2/arduino-usbserial/Arduino-usbserial-atmega16u2-Uno-Rev3.hex
  - `avrdude -p at90usb82 -F -P usb -c avrispmkii -U flash:w:UNO-dfu_and_usbserial_combined.hex -U lfuse:w:0xFF:m -U hfuse:w:0xD9:m -U efuse:w:0xF4:m -U lock:w:0x0F:m`
