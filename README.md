Forked and modified from https://github.com/Grawp/rtl8812au_rtl8821au

# Dangerous Modifications
Added {USB_DEVICE(0x7392, 0xA812),.driver_info = RTL8821}, /* Edimax - Edimax */ to the recognized USB_DEVICE list for the driver to for it to recognize the Edimax AC USB WiFi dongle model EW-7811UTC.

Although this works for me, use this at your own risk.  I don't know why the 4.3 driver train dropped support for this particular USB dongle, but this hack does appear to 'work' -- That is it correctly recognizes and loads the module and the USB dongle works based on preliminary observations.

Successful compile was on 4.4.1-2-ARCH #1 SMP PREEMPT x86_64 GNU/Linux
