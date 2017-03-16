I made a MSX1 core, with a SCC Megaram from OCM. Specifications:

- MSX1 USA, 60Hz vertical frequency.
- 128K RAM Mapper.
- 128K Nextor (MSX-DOS2 evolution) ROM with SD driver.
- 256K of RAM to Megaram SCC/SCC+ from OCM project.
- Keyboard PT-BR layout (for a while).
- Simple switched I/O ports (no software yet).
- Multiple boards, incluing ZX-Uno.
- CVBS video only, no scandoubler yet.

The binaries are located here:

https://drive.google.com/drive/folders/0B5wpc_jDN_n0Z1BvSms2YWJHWGc

Format a SD Card in FAT16 (4GB max) and unzip the 'msx1_sd_files.zip' file in SD card root.

The MSX 1 FPGA contains a IPL loader to clear the RAM and load the 'NEXTOR.ROM' SD file to RAM. The ROM is implemented in Xilinx BlockRAM.

CTRL+ALT+DEL is soft reset, CTRL+ALT+F12 is hard reset (run IPL again) and CTRL+ALT+BACKSPACE is ZX-Uno Standard, reload first core from SPI Flash.

The joystick port is mapped to JoyMega, configure the ZX-Uno hardware to SEGA Genesis joypad.

To load ROM in SCC Megaram, uses the ROMLOAD.COM (it is in SD files) with '/S' switch for starting:

ROMLOAD game.rom /S

The core is in beta stage yet, sources will be released soon.

Thanks.