# AltiduoSMT
SMT version of the AltiDuo Mini. Warning! Not all components can be soldered by hand.
Firmware for the [AltiDuo Mini SMT](http://rocket.payload.free.fr/index.php?option=com_content&view=article&id=26&Itemid=15&lang=en) altimeter using an ATtiny 84  microcontroller
This is another version of the Alti Duo that is using an Attiny 84 processor. It is smaller than the other AltiDuo that is using an ATMega 328. However unlike the big AltiDuo it cannot connect to the USB port. You cannot remove the ship so it cannot be re-programmed. The ship is programmed before you solder it.

<img src="/pictures/AltiDuoSMT-top.JPG" width="49%"> <img src="/pictures/AltiDuoSMT-bottom.JPG" width="49%">

# Building the code
You will need to download the Arduino ide from the [Arduino web site](https://www.arduino.cc/).
You need to download the [Attiny support](https://code.google.com/archive/p/arduino-tiny/downloads) and install it to your Arduino environement.
You have to load the Arduino Attiny84 boot loader to your ATtiny84 micro controller. 
Make sure that you download the following [support libraries](https://github.com/bdureau/AltimetersLibs) tinyBMP085, tinyWireM, tinyWireS and copy them to the Arduino library folder. To compile it you need to choose the Attiny 84 and the correct USB port.
You will need to use an AVR programmer and an adapter to program the microcotroller, refer to the documentation.

# Using other pressure sensors
Unfortunatly it is not possible to use a bmp280 sensor, I have ported the library but unfortunatly the attiny 85 has not enought on board memory.
