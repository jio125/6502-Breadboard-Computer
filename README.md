# 6502 Based breadboard computer

Breadboard computer based around the 6502 microprocessor using Ben Eaters architecture

## Parts

- 65c02 microprocessor
- 65c22 Versatile Interface Adapter
- 28C256 EEPROM
- 62256 SRAM
- LCD Display

## Support software

Assembled using vasm assembler

EEPROM programmed using TommyPROM arduino based programmer

## Reference steps

### Programming EEPROM

1. Connect programmer to computer via USB and inster EEPROM into breadboard
2. Launch minicom from terminal with the appropriate serial port. ex: `minicom -D /dev/tty.usbserial-1431340`
3. In TommyPROM interface send command `W0` to write EEPROM (may need to unlock EEPROM with `U` command first)
4. Press `CTRL-I` then `S` to send file using xmodem, follow the onscreen promts to select and send the appropriate binary file
