# Spellboard Firmware Info

- Firmware: [QMK](https://docs.qmk.fm/)
- Keyboard Maintainer: [crkalapat](https://github.com/crkalapat)
- Hardware: [Seeed Studio XIAO RP2040](https://www.seeedstudio.com/XIAO-RP2040-v1-0-p-5026.html)

## Building New Firmware

To flash the XIAO with the QMK Firmware, you can either directly use the .uf2 file in the repository or generate your own from QMK files.

To generate your own .uf2 file, copy the `/firmware/spellboard/` directory into your local directory `/qmk-firmware/keyboards/`. Ensure sure that [QMK is properly installed](https://docs.qmk.fm/newbs_getting_started) beforehand. In the terminal, run the command

```
qmk compile -kb spellboard -km default
```

to generate a .uf2 file to flash on the XIAO.

## Flashing Firmware

Once you have a .uf2 file to flash onto the XIAO, enter the bootloader by pressing and holding on the _B_ button on the front of the XIAO. From there, you can add the .uf2 file to the XIAO.
