# mega_flashlight_public
Renders for the preliminary design of rev2.5 in Fusion 360


## Overview
The MegaFlashlight is shown here with a 230Wh external battery and a large 2° CPC to illustrate the modular nature of the design.

![alt text](https://github.com/benhogervorst/mega_flashlight_public/blob/main/design/renders_rev2.5/iso-cpc-230wh_battery.png?raw=true)
![alt text](https://github.com/benhogervorst/mega_flashlight_public/blob/main/design/renders_rev2.5/side-cpc-230wh_battery.png?raw=true)
![alt text](https://github.com/benhogervorst/mega_flashlight_public/blob/main/design/renders_rev2.5/iso.png?raw=true)
![alt text](https://github.com/benhogervorst/mega_flashlight_public/blob/main/design/renders_rev2.5/side.png?raw=true)


## End Attachment mounting
Mounting for end attachments like CPCs and lenses is done using a square M3 hole layout for mounting, or clips on the corners.  
The CPC shown above uses M3 screws for mounting, but the lens shown below uses clips

![alt text](https://github.com/benhogervorst/mega_flashlight_public/blob/main/design/renders_rev2.5/front.png?raw=true)
![alt text](https://github.com/benhogervorst/mega_flashlight_public/blob/main/design/renders_rev2.5/front_lens.png?raw=true)
![alt text](https://github.com/benhogervorst/mega_flashlight_public/blob/main/design/renders_rev2.5/iso_lens.png?raw=true)


## Bottom Attachment mounting
Batteries and other attachments can be mounting to the bottom of the flashlight using the modular slide mechanism.
The orange battery shown in some renders uses this slider mount to allow it to slide and lock onto the flashlight.
There is a smal latch at the front of the flashlight that allows attachments to be removed.

![alt text](https://github.com/benhogervorst/mega_flashlight_public/blob/main/design/renders_rev2.5/bottom_iso2.png?raw=true)
![alt text](https://github.com/benhogervorst/mega_flashlight_public/blob/main/design/renders_rev2.5/bottom_iso.png?raw=true)
![alt text](https://github.com/benhogervorst/mega_flashlight_public/blob/main/design/renders_rev2.5/bottom.png?raw=true)


## Rear I/O
The flashlight has two rear I/O ports - an XT-60 connector for power input and a USB-C port for programming the built in microcontroller.

![alt text](https://github.com/benhogervorst/mega_flashlight_public/blob/main/design/renders_rev2.5/rear.png?raw=true)


## Internal Layout and Design
The MegaFlashlight is designed around an old Intel Reference design CPU heatsink and 80mm fan.  
The 100W LED is mounted using an adapter bracket to the thermal contact point of the heatsink.  
The fan is reversed to draw air through the sides of the enclosure, across the fins, and out the back (top of the heatsink) towards the rear of the flashlight.
Air traveling from the LED heatsink fins then passes over the boost converter in the top portion of the rear enclosure before being blown out the vent in the back.

![alt text](https://github.com/benhogervorst/mega_flashlight_public/blob/main/design/renders_rev2.5/side-section_analysis.png?raw=true)

## Power
Batteries and specifc methods for powering the MegaFlashlight aren't covered in depth in this repo, but the power draw specs and my currently implemented battery are mentioned below.
The flashlight is designed to take 10-16v into the rear XT-60 connector.  Max power draw is around 120W, or about 10A at 12v at full load, with some safety net.
The battery shown below uses 24 18650 cells configured in a 3S 8P configuration, netting a nominal voltage of about 12.6v.
The top of the battery includes the sliding rails which mount and clip it into place securely on the bottom of the flashlight.

![alt text](https://github.com/benhogervorst/mega_flashlight_public/blob/main/design/renders_rev2.5/battery.png?raw=true)

## Software and Electrical Hardware
These aspects of this design will be discussed later on a different page.


## Further improvements
There are quite a few things that could be improved on this design, which are described below:
- Better status indication using a screen or LEDs
- Improved software for handling trigger pressing/holding (currently in progress)
- Better internal support for ESP32 so that plugging in USB-C doesn't break it loose inside the casing
- More support for threadcerts in the front for internal mounting of the heatsink
- Would like to add voltage monitoring for the ESP32 to monitor the battery voltage
- Could at some point like to add wifi/web interface functionality for additional debugging and configuration


## Additional renders
Below are some internal wireframe renders that show the layout of the flashlight.
![alt text](https://github.com/benhogervorst/mega_flashlight_public/blob/main/design/renders_rev2.5/iso_wireframe.png?raw=true)
![alt text](https://github.com/benhogervorst/mega_flashlight_public/blob/main/design/renders_rev2.5/front_wireframe.png?raw=true)
![alt text](https://github.com/benhogervorst/mega_flashlight_public/blob/main/design/renders_rev2.5/side_wireframe.png?raw=true)
![alt text](https://github.com/benhogervorst/mega_flashlight_public/blob/main/design/renders_rev2.5/top_wireframe.png?raw=true)
