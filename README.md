atmega16u2-adc
==============
- https://github.com/dirkarnez/ringbuffer
- https://github.com/dirkarnez/lufa-playground

### Datasheet
- https://ww1.microchip.com/downloads/en/DeviceDoc/doc7799.pdf

### Notes
- `"%LOCALAPPDATA%\Arduino15\packages\arduino\tools\avrdude\6.3.0-arduino17/bin/avrdude" "-C%LOCALAPPDATA%\Arduino15\packages\arduino\tools\avrdude\6.3.0-arduino17/etc/avrdude.conf" -v -p atmega16u2 -carduino -PCOM5 -U flash:w:Keyboard.hex:i -F`


### Reference
- [analogRead() - Arduino Reference](https://www.arduino.cc/reference/en/language/functions/analog-io/analogread/)
- https://github.com/arduino/ArduinoCore-avr/blob/master/firmwares/atmegaxxu2/arduino-usbserial/Arduino-usbserial-atmega16u2-Uno-Rev3.hex
  - `avrdude -p at90usb82 -F -P usb -c avrispmkii -U flash:w:UNO-dfu_and_usbserial_combined.hex -U lfuse:w:0xFF:m -U hfuse:w:0xD9:m -U efuse:w:0xF4:m -U lock:w:0x0F:m`
