# Systems

This outlines how to add support for many different systems into EmulationStation through configuration of `es_systems.cfg`.

##	Arcade Systems configration

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
## Super Nintendo Entertainment System
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
## Nintendo 64
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
## Nintendo DS
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
## Nintendo Gamecube
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
