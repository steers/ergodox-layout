# steers' Infinity ErgoDox Layout
This is the current layout I'm using day-to-day on my Infinity ErgoDox keyboard.
There are many like it, but this one is mine. Feel free to fork and make it yours.

## Using This Layout
1. Paste the [json layout](https://github.com/steers/ergodox-layout/blob/master/MDErgo1-Default.json) into
the [Input Club Configurator](https://input.club/configurator-ergodox)
1. Make any tweaks you want to make.
1. Click `download firmware` to generate DFU firmware files from your layout (`.zip` archive)
1. [Follow the documentation](https://github.com/kiibohd/controller/wiki/Loading-DFU-Firmware) for your platform
to flash the firmware to each half of your board separately.

### Flashing on Linux
In the firmware archive, the following files should exist:
```
$ ls *.bin
left_kiibohd.dfu.bin  right_kiibohd.dfu.bin
```

Disconnect both halves of the keyboard, then for each half in turn:

1. Connect the keyboard half directly via USB3 A-B
1. Hit the flash button on the keyboard (may need a pencil/paperclip)
1. `sudo dfu-util -D ${bin}`
