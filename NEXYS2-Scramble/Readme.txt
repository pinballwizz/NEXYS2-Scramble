Scramble for the NEXYS2-500 Dev Board.

Notes:
Setup for 1 player arcade controls (8 switches) (coin-start-up-down-left-right-shoot-bomb).
Each switch is connected one side to NEXYS2 I/O Pin and other side to VCC 3.3v (pins 6 or 12 on GPIO Pin Headers).
Pin Header locations are specified in the "SCRAMBLE_TOP.ucf" File.
Audio output is pin4 on JA Header. See instructions in the "dac.vhd" file for connecting audio to ext amp/spkr.

Build:
* Obtain correct roms file for stern scramble "scrambles.zip".
* Unzip rom files to stern_scramble folder inside the roms folder.
* Run the build roms script in the scripts folder.
* Open the NEXYS2-Scramble project file using Xilinx 11.1 webpack or similar and compile.
* Generate Programming file with startup options set to use JTAG Clock.
* Program NEXYS2 Board using Adept and the BIT file generated by XILINX Webpack.
