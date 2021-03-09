# WM8731PMOD

A small board to extend audio capabilities to FPGA via PMOD interface. Designed with [lceda](https://lceda.cn)。

It includes:

1. [WM8731](https://www.cirrus.com/products/wm8731/) chip with I2C and I2S
2. [PAM8303](https://m5stack.oss-cn-shenzhen.aliyuncs.com/resource/docs/datasheet/hat/PAM8303_en.pdf) + XH2.54 2P for speaker output
3. 4x TRS port for line in, mic in, line out and headphone out
4. [PMOD](https://reference.digilentinc.com/_media/reference/pmod/pmod-interface-specification-1_2_0.pdf) connection to FPGA

## PMOD pin definition

| Description  | Pin number | Pin number | Description |
| ------------ | ---------- | ---------- | ----------- |
| SPEAKER_MUTE | 1          | 2          | I2S_LRCLK   |
| MCLK         | 3          | 4          | I2S_DACDAT  |
| I2C_SCL      | 5          | 6          | I2S_ADCDAT  |
| I2C_SDA      | 7          | 8          | I2S_BCLK    |
| GND          | 9          | 10         | GND         |
| VCC          | 11         | 12         | VCC         |


## Project

Online version is available at [oshwhub.com/jiegec/wm8731mod](https://oshwhub.com/jiegec/wm7831pmod)。

Schematic, PCB, Gerber and BOM files are included in this repo.

![Schematic](Schematic.png)

![PCB](PCB.png)

## References

- [A similar project](http://ebrombaugh.studionebula.com/synth/codec_pmod/index.html)
- [DE2 board schematic](https://wiki.bu.ost.ch/infoportal/_media/fpga/cyclone_iv/de2_115_schematic.pdf)

## License

Licensed under CERN-OHL-P.