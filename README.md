# Tutorial

aml_autoscript

if printenv bootfromsd; then exit; fi;
if fatload mmc 0 0x1000000 u-boot.ext; then go 0x1000000; fi;

boot.ini

if test "${devtype}" = ""; then setenv devtype "/dtb/amlogic/meson-gxl-s905x-p212.dtb"; fi
if fatload ${devtype} ${devnum} 0x1000000 u-boot.ext; then go 0x1000000; fi;

partisi bootloader di sdcard ganti pakai punya hg jangan bawaan firmware

# Tested Device
- HG680P

# Suppport Me
https://saweria.co/vincher
