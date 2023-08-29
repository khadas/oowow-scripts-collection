# oowow-scripts-collection

Create autoinstall image http://docs.khadas.com/software/oowow/how-to/oowow-autoinstall-disk

## Download

https://raw.githubusercontent.com/khadas/oowow-scripts-collection/main/autoinstall-disk-create-oowow

    cd
    wget https://raw.githubusercontent.com/khadas/oowow-scripts-collection/main/autoinstall-disk-create-oowow

## Build and Write Autoinstallation disk

    [DISK=/dev/sdX] bash ./autoinstall-disk-create-oowow [IMAGE [/dev/sdX]]

## Headless usage

All process can going in auto mode without any user action! After
installation process will be done user must remove installation disk and
reboot device! User can control all states by led indication.

## LED indication

### Edge2

OOWOW version >= 230828

    START          : sys_led WHITE heartbeat
    WRITE/PROGRESS : sys_led WHITE blink      + mcu_led RED blink
    ERROR          : sys_led RED   solid      + mcu_led WHITE heartbeat
    DONE           : sys_led WHITE slow blink + mcu_led WHITE solid
