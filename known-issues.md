## Motorola One (deen)
- Encryption:
  - We can even use encryption in AOSP, but the recovery used [(twrp/ofox)](https://github.com/jro1979oliver/device_motorola_deen/releases) doesn't decrypt, so I keep it disabled.
- Slot swap:
  - In the AOSP recovery process, it doesn't update the slot from A to B, only from B to A, for some unknown reason.
  - In these cases, you can return to the bootloader and use the command "fastboot --set-active=b" and return to recovery mode.
  - In the available twrp/ofox recovery versions, the slot swapping function works correctly.

## Motorola G6 Play (al/jeter)
- Encryption:
  - We could also use AOSP encryption, but the [TWRP](https://sourceforge.net/projects/jeter-builds/files/twrp-3.7.0_9.0.img/download) we're using doesn't support encryption due to the small partitions, so we keep it disabled.
