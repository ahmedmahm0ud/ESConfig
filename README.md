# Systems

This outlines how to add support for many different systems into EmulationStation through configuration of [`es_systems.cfg`](https://github.com/lucifer-1/ESConfig/blob/master/emulationstation/es_systems.cfg).

##  Arcade Systems configration

### Multiple Arcade Machine Emulator
``` xml
  <system>
    <name>mame</name>
    <fullname>Multiple Arcade Machine Emulator</fullname>
    <path>~/.emulationstation/roms/mame/</path>
    <extension>.zip .chd</extension>
    <command>retroarch -f -L ~/.config/retroarch/cores/mame_libretro.so %ROM%</command>
    <platform>mame</platform>
    <theme>mame</theme>
  </system>
```
### Neo Geo
``` xml
  <system>
    <name>neogeo</name>
    <fullname>Neo Geo</fullname>
    <path>~/.emulationstation/roms/neogeo/</path>
    <extension>.zip</extension>
    <command>retroarch -f -L ~/.config/retroarch/cores/fbneo_libretro.so %ROM%</command>
    <platform>neogeo</platform>
    <theme>neogeo</theme>
  </system>
```
## Nintendo Systems configration

### Nintendo Entertainment System
``` xml
  <system>
    <name>nes</name>
    <fullname>Nintendo Entertainment System</fullname>
    <path>~/.emulationstation/roms/nes/</path>
    <extension>.zip .nes .smc .sfc .fig .swc .mgd</extension>
    <command>retroarch -f -L ~/.config/retroarch/cores/nestopia_libretro.so %ROM%</command>
    <platform>nes</platform>
    <theme>nes</theme>
  </system>
```
### Super Nintendo Entertainment System
``` xml 
  <system>
    <name>snes</name>
    <fullname>Super Nintendo Entertainment System</fullname>
    <path>~/.emulationstation/roms/snes/</path>
    <extension>.zip .smc .sfc .fig .swc</extension>
    <command>retroarch -f -L ~/.config/retroarch/cores/snes9x_libretro.so %ROM%</command>
    <platform>snes</platform>
    <theme>snes</theme>
  </system>
```
### Nintendo 64
``` xml
  <system>
    <name>n64</name>
    <fullname>Nintendo 64</fullname>
    <path>~/.emulationstation/roms/n64/</path>
    <extension>.v64 .zip .n64 .z64 .bin</extension>
    <command>retroarch -f -L ~/.config/retroarch/cores/mupen64plus_next_libretro.so %ROM%</command>
    <platform>n64</platform>
    <theme>n64</theme>
  </system>
```
### Nintendo DS
``` xml
  <system>
    <name>nds</name>
    <fullname>Nintendo DS</fullname>
    <path>~/.emulationstation/roms/nds</path>
    <extension>.nds .bin .7z</extension>
    <command>retroarch -f -L ~/.config/retroarch/cores/desmume_libretro.so %ROM%</command>
    <platform>nds</platform>
    <theme>nds</theme>
  </system>
```
### Nintendo Gamecube
``` xml
  <system>
    <name>gc</name>
    <fullname>Nintendo Gamecube</fullname>
    <path>~/.emulationstation/roms/gc/</path>
    <extension>.iso .zip .elf .dol .wad .gcm</extension>
    <command>dolphin-emu -b --exec %ROM%</command>
    <platform>gc</platform>
    <theme>gc</theme>
    <!-- For running properly, the Dolphin core requires to have the Dolphin Sys folder in the proper location. After downloading the core within RetroArch, execute the following steps: "https://docs.libretro.com/library/dolphin/" -->
  </system>
```
## Nintendo's GameBoy Systems configration

### Game Boy
``` xml
  <system>
	<name>gb</name>
	<fullname>Game Boy</fullname>
	<path>~/.emulationstation/roms/gb/</path>
	<extension>.gb .zip</extension>
	<command>retroarch -f -L ~/.config/retroarch/cores/gambatte_libretro.so %ROM%</command>
	<platform>gb</platform>
	<theme>gb</theme>
  </system>
```
### Game Boy Color
``` xml
  <system>
	<name>gbc</name>
	<fullname>Game Boy Color</fullname>
	<path>~/.emulationstation/roms/gbc/</path>
	<extension>.gbc .zip</extension>
	<command>retroarch -f -L ~/.config/retroarch/cores/gambatte_libretro.so %ROM%</command>
	<platform>gbc</platform>
	<theme>gbc</theme>
  </system>
```
### Game Boy Advance
``` xml
  <system>
	<name>gba</name>
	<fullname>Game Boy Advance</fullname>
	<path>~/.emulationstation/roms/gba/</path>
	<extension>.gba .zip</extension>
	<command>retroarch -f -L ~/.config/retroarch/cores/mgba_libretro.so %ROM%</command>
	<platform>gba</platform>
	<theme>gba</theme>
  </system>
```
## Sega Systems configration

### Sega Genesis
``` xml
  <system>
	<name>genesis</name>
	<fullname>Sega Genesis</fullname>
	<path>~/.emulationstation/roms/genesis/</path>
	<extension>.smd .bin .gen .md .sg .zip</extension>
	<command>retroarch -f -L ~/.config/retroarch/cores/genesis_plus_gx_libretro.so %ROM%</command>
	<platform>genesis</platform>
	<theme>genesis</theme>
  </system>
```
### Sega Mega Drive
``` xml
  <system>	
	<name>megadrive</name>
	<fullname>Sega Mega Drive</fullname>
	<path>~/.emulationstation/roms/megadrive/</path>
	<extension>.smd .bin .gen .md .sg .zip</extension>
	<command>retroarch -f -L ~/.config/retroarch/cores/genesis_plus_gx_libretro.so %ROM%</command>
	<platform>megadrive</platform>
	<theme>megadrive</theme>
  </system>
```
### Sega Master System
``` xml
  <system>
	<name>mastersystem</name>
	<fullname>Sega Master System</fullname>
	<path>~/.emulationstation/roms/mastersystem/</path>
	<extension>.sms</extension>
	<command>retroarch -f -L ~/.config/retroarch/cores/genesis_plus_gx_libretro.so %ROM%</command>
	<platform>mastersystem</platform>
	<theme>mastersystem</theme>
  </system>
```
### Sega Game Gear
``` xml
  <system>
	<name>gamegear</name>
	<fullname>Sega Game Gear</fullname>
	<path>~/.emulationstation/roms/gamegear/</path>
	<extension>.gg</extension>
	<command>retroarch -f -L ~/.config/retroarch/cores/genesis_plus_gx_libretro.so %ROM%</command>
	<platform>gamegear</platform>
	<theme>gamegear</theme>
  </system>
```
### Sega CD
``` xml
  <system>
	<name>segacd</name>
	<fullname>Sega CD</fullname>
	<path>~/.emulationstation/roms/segacd/</path>
	<extension>.cue .iso</extension>
	<command>retroarch -f -L ~/.config/retroarch/cores/genesis_plus_gx_libretro.so %ROM%</command>
	<platform>segacd</platform>
	<theme>segacd</theme>
  </system>
```
### Sega 32X
``` xml
  <system>
	<name>sega32x</name>
	<fullname>Sega 32X</fullname>
	<path>~/.emulationstation/roms/sega32x/</path>
	<extension>.32x .smd .bin .md .zip</extension>
	<command>retroarch -f -L ~/.config/retroarch/cores/picodrive_libretro.so %ROM%</command>
	<platform>sega32x</platform>
	<theme>sega32x</theme>
  </system>
```
### Sega Saturn
``` xml
  <system>
	<name>saturn</name>
	<fullname>Sega Saturn</fullname>
	<path>~/.emulationstation/roms/saturn/</path>
	<extension>.cue .nrg .zip .bin .iso .mdf</extension>
	<command>retroarch -f -L ~/.config/retroarch/cores/mednafen_saturn_libretro.so %ROM%</command>
	<platform>saturn</platform>
	<theme>saturn</theme>
  </system>
```
### Sega Dreamcast
``` xml
  <system>
	<name>dreamcast</name>
	<fullname>Sega Dreamcast</fullname>
	<path>~/.emulationstation/roms/dreamcast/</path>
	<extension>.cdi .gdi</extension>
	<command>retroarch -f -L ~/.config/retroarch/cores/flycast_libretro.so %ROM%</command>
	<platform>dreamcast</platform>
	<theme>dreamcast</theme>
  </system>
```

## PlayStation Systems configration

### PlayStation
``` xml
  <system>
	<name>psx</name>
	<fullname>PlayStation</fullname>
	<path>~/.emulationstation/roms/psx/</path>
	<extension>.cue .cbn .img .iso .m3u .mdf .pbp .toc .z .znx .PBP</extension>
	<command>retroarch -f -L ~/.config/retroarch/cores/mednafen_psx_hw_libretro.so %ROM%</command>
	<platform>psx</platform>
	<theme>psx</theme>
	<!-- For running properly you should have these "scph5500.bin","scph5501.bin" and "scph5502.bin" BIOS files placed into the ‘system’ folder of Retroarch "~/.config/retroarch/system/" and roms directory. Required to make games work -->
  </system>
```
### PlayStation 2
``` xml
  <system>
	<name>ps2</name>
	<fullname>PlayStation 2</fullname>
	<path>~/.emulationstation/roms/ps2/</path>
	<extension>.iso .img .bin .mdf .z .z2 .bz2 .dump .cso .ima .gz</extension>
	<command>retroarch -f -L ~/.config/retroarch/cores/play_libretro.so %ROM%</command>
	<platform>ps2</platform>
	<theme>ps2</theme>
	</system>
```
### PlayStation Portable
``` xml
  <system>
	<name>psp</name>
	<fullname>PSP</fullname>
	<path>~/.emulationstation/roms/psp/</path>
	<extension>.cso .iso .pbp .PBP</extension>
	<command>retroarch -f -L ~/.config/retroarch/cores/ppsspp_libretro.so %ROM%</command>
	<platform>psp</platform>
	<theme>psp</theme>
	<!-- The PPSSPP core requires assets files to be fully functional. Assets such as fonts and backgrounds that are required for memory card screens. You can simply follow this tutorial at "https://docs.libretro.com/library/ppsspp/" -->
  </system>
```
