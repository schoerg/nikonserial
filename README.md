# nikonserial
Research on the serial protocol used in Nikon film cameras like the F100.

# What?

Some Nikon film cameras (like F5, F6, F100 ...) allow you to save settings (ISO, aperture, lens ...) for each shot to an internal storage. You can compare that to modern EXIF metadata, but it's not the same technically. Nikon also sold an external device to save that data onto a CF card called MV-1. It's now very hard to get such a thing for a reasonable price.

# Why?

If you digitalise your film rolls you won't have that data anymore but the settings used by your scanner/camera. If you have written down your settings for each shot you can manually edit the EXIF data to show the "proper" value.

# How?

The Nikon cameras in question have a 10-pin connector used for remote releases. It also features a TTL serial port. Voltage levels are at 5V.
Documentation about the serial port is not readily available, you can see some links in the last section. There are tools available for readout like "Camera Companion" and SoftTALK. Both are closed source programs. I have not found a Linux (or open source alternative).

# Hardware

There is no need to buy special hardware, a cheap FTDI or similar USB-to-Serial device will work. Connect RX to TX and vice versa and GND to GND. If you have a voltage selector, use 5V. 3V3 might work, it did not for me.

# Interesting links

https://www.kenrockwell.com/nikon/f6.htm#mv1

http://www.holymoose.com

https://www.cocoon-creations.com/COCOON-NiCommSoftTALK-98.shtml

https://www.flickr.com/photos/fabbiomenna/8603276421/in/photostream/

https://www.schneordesign.com/diy/diy-photography/mc-30/

http://www.mir.com.my/rb/photography/hardwares/classics/NikonF5/accessories/PhotoSecretary/index.htm

http://web.archive.org/web/19981207005100/http://members.aol.com/khancock/pilot/nbuddy/protocol.html
