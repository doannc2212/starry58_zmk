# Starry58 firmware

Supermini nRF52840

### Pinout mapping

To ensure proper firmware operation, accurately connect the pins according to the pinout diagram below.

![Pinout](assets/pinout.png?raw=true "GPIO Mapping")

### Enter bootloader mode
The Supermini nRF52840 may need to have RST shorted to GND twice, quickly to actually jump to bootloader
![Bootloader](assets/bootloader.png?raw=true "Bootloader")

## Flash firmware

1. Go to actions tab on github repository
2. Download action output (firmware.zip)
3. Enter bootloader mode of Supermini nRF52840, then a drive named NICE_NANO will appear in explorer
4. Extract firmware.zip file and paste `settings_reset.uf2` to root directory NICE_NANO disk. USB will be eject.
5. Enter bootloader mode again.
6. Paste `<firmware name>_left.uf2` or `<firmware name>_right.uf2` to NICE_NANO drive, depend on which split side plugged-in.

### Repeat step 4-6 to other part.

Now you can find a bluetooth device named **Starry58 (Left)**
