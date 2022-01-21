# DIY-Keyboard
## Designing a complete keyboard mainly for ISO-DE users. 

### Planned layouts:
- [ ] ISO
- [ ] ANSI
 
### Planned sizes:
- [ ] TKL
- [ ] TKL without F row
- [ ] 65%

### Planned Connection:
- [ ] USB-C

### Planned Features:
- [ ] Switch Plate
- [ ] Rotary Encoder
- [ ] Hot Swap
- [ ] Maybe Display? 
- [ ] QMK
- [ ] RGB per Key?
- [ ] RGB stripes like GMMK PRo
- [ ] fingerprint sensor?

### Planned designen functional Case, feel free to design your own with provided schematics. 

### Maybe worth trying
- [ ] Programming GUI to controll Keyboard


# Choosing a Controller:<br/>
We choose 3 controllers from all of the QMK supported ones (https://github.com/qmk/qmk_firmware/blob/master/docs/compatible_microcontrollers.md).  
We chose them, because they are available, have enough flash and have enough GPIOs.
The last two are ment to be used for per key RGB, because you will need way more GPIO pins that non per key illumination. 
<br/>
## AT90USB646-MUR:
Flash: 64kB, IO: 48:
https://www.mouser.at/ProductDetail/Microchip-Technology-Atmel/AT90USB646-MUR?qs=rBGENRD8NwIhZgS5YIDA9Q%3D%3D
<br/> 
Important pages from the datasheet:
https://www.mouser.at/datasheet/2/268/doc7593-1369068.pdf
Quratz configuration on page 43

## STM32G474VET6:
Flash: 512 kB, IO: 107
https://www.mouser.at/ProductDetail/STMicroelectronics/STM32G474VET6?qs=sGAEpiMZZMv0NwlthflBiw1pCvrEn%252BxK6MfMEmRsg98%3D
<br/>

## STM32F446ZET7
Flash: 512KB, IO: 14
https://www.mouser.at/ProductDetail/STMicroelectronics/STM32F446ZET7?qs=sGAEpiMZZMsKEdP9slC0YW7w0sAsT3%2FGB%2FjI7C9YUKU%3D

# Stuff to remember:
CNC-Parts: https://spanflug.de/<br/>
Switch-Plate Generator: https://kbplate.ai03.com/

STM32:<br/>
USB Pins: PA11 = DM, PA12 = DP;

Voltage Regulator : TC1264