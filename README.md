# sys-botbase based on jakibakis sys-netcheat
The purpose of this sys-module is to allow users to remote control their switch via wifi connection as well as to read and write to a games memory.
This work is presented to work with Animal Crossing - New Horizons, for public in-game online sessions.

## Warning:
Don't even think of blaming me if anything goes wrong with you using this. It's supposed to help you in the development of bot automation, but I am not liable for any damages or bans you might get in the process. Use at your own risk and all that.

## (planned) feature list:
### button input:
- [x] simulate button press
- [x] simulate button hold
- [x] set complete controller state

### touchscreen input:
- [ ] simulate touchscreen press
- [ ] simulate touchscreen hold
- [ ] simulate touchscreen drawing

### Memory reading:
- [ ] read x bytes of consecutive memory from RAM based on absolute memory address
- [x] read x bytes of consecutive memory from RAM based on address relative to heap base

### Memory writing:
- [ ] write x bytes of consecutive memory to RAM based on absolute memory address
- [x] write x bytes of consecutive memory to RAM based on address relative to heap base

### screen capture:
- [ ] capture current screen and send it 

# Installation
I've only tried this on Atmosphere (0.10.2), so if you are using a different cfw your experience might vary.

Copy the sys-botbase.nsp file to sdmc://atmosphere/contents/430000000000000B and rename it to exefs.nsp.
Create a new folder in sdmc://atmosphere/contents/430000000000000B names "flags".
Create a empty file called boot2.flag inside this folder.
Restart your switch.

The sysmodule opens a socket connection on port 6000. See the python example on how to talk to the sysmodule and what commands are available.


# big thank you to jakibaki for a great sysmodule base to learn and work with, as well as being helpful on the Reswitched discord!
# Thanks to the original dev for this bot module, and to some other developers as well.
