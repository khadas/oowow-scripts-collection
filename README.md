# oowow-scripts-collection

Create autoinstall image

## USAGE

    [DISK=/dev/sdX] ./autoinstall-disk-create-oowow [IMAGE [DISK]]

## Headless

Remove installation disk for reboot

## LED indication

### Edge2

OOWOW version >= 230828

* START : sys_led WHITE heartbeat
* WRITE : sys_led WHITE blink      + mcu_led RED blink
* ERROR : sys_led RED   solid      + mcu_led WHITE heartbeat
* DONE  : sys_led WHITE slow blink + mcu_led WHITE solid

