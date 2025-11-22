# diskoteket/3x3macropad

* Keyboard Maintainer: [diskoteket](https://github.com/diskoteket)
* Hardware Supported: *RP2040-Zero*
* Hardware Availability:
  * [Amazon](https://www.amazon.se/Hailege-RP2040-Zero-Development-mikrokontroll-dubbelk%C3%A4rnig/dp/B0CJY3CDVY)

## Building the firmware
Clone this repo
```bash
git clone git@github.com:Diskoteket/qmk_firmware.git
```

Build the firmware using docker
```bash
util/docker_build.sh diskoteket/3x3macropad:via
```

## Flashing the firmware
Hold the bootcell button while plugging in the controller via usb
```bash
cp .build/diskoteket_3x3macropad_via.uf2 /run/media/<user>/RPI-RP2
``` 

## Configuring the keyboard
1. Go to [Via](https://www.usevia.app/)
2. Navigate to **Settings**
3. Enable the setting `Show Design Tab`
4. Navigate to **Design** and upload `via.json`
5. Navigate to **Configure**
6. Configure the keymap and enjoy the macropad.
