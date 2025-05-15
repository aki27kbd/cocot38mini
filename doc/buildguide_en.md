# Build Guide

![cocot38mini_main02](/images/main_02.jpg)

This is a buildguide for cocot38mini v2.  
For v1 buildguide, refer to the previous documents ([JP](v1/buildguide.md) / [EN](v1/buildguide_en.md))

cocot38mini is designed as a more compact version of cocot series, with column-staggered 38 keys, 25mm trackbvall and 3D printed case. To begin with, please make sure you read this buildguide carefully and you have everything you need before you start to asseble.


## Parts
### Parts Included

|Parts|Qty|Notes|
|---|---|---|
|PCB|1||
|Sensor PCB|1||
|Sensor (PMW3360)|1||
|Rubber Feet|4||
|Zirconia Balls (2mm)|3||


### Additional Required Parts

|Parts|Qty|Notes|
|---|---|---|
|3D Printed Case (Top+Bottom)|1|You can download 3d data to order 3d printing service by yourself|
|Keyswitch|37 or 38|MX|
|Keycap|37 or 38|MX|
|Rotary Encoder + Knob |1|Optional|
|Spring Pin Header or Pin Header (H2.5mm)|At least 20 pins are necessary||
|25mm Trackball|1||
|Bearing Roller|3|Optional (Bearing Roller Support)|
|Tadpole|8|Optional (Tadpole Mount)|
|Heated Insert Nut|8|Optional (Top Mount)|
|M2 Screw 3mm|8|Optional (Top Mount)|
|USB-Type C Cable|1||


## Assembly
### Parts Check

  First, please make sure that you have all the parts listed above. If the PCB comes with tabs, break off the tabs and lightly file the cut surfaces.

### Firmware

  It is delivered with the default firmware is written. Before starting soldering, make sure you confirm the sensor PCB is recognized as cocot38mini when you plug USB to it.

  If you wish to write your own firmware, please follow the instructions below.

  - Press the RESET button (SW39) while holding down the BOOT button (SW40) on the bottom side to enter boot loader mode.
  - The firmware is written by dragging and dropping the [.uf2](https://github.com/aki27kbd/cocot38mini/blob/main/firmware/aki27_cocot38mini_vial.uf2) file into the drive named RPI-RP2.  
  ![cocot38mini_bg_](/images/bg_firmware.jpg)  


  Keymap is editable from [vial](https://vial.rocks/).  
  You can confirm that trackball and LEDs are working correctly with this firmware. You can confirm the trackball move after you assemble the following steps.

  ![vial](/images/vial.jpg)

  The default firmware enables "Auto Mouse Layer", with which you can automatically jump into a specific mouse layer when you move trackball. You can toggle on/off this function with the custom keycode `AM_TOG`.

  The source code is available [here](https://github.com/aki27kbd/vial-qmk/tree/vial/keyboards/aki27/cocot38mini).

### Sensor PCB

  Place the mouse sensor (PMW3360) on the sensor board in the orientation shown in the picture. Please make sure to align the ● mark on the silk with the ● mark on the board.
  ![cocot38mini_bg_](/images/bg_pmw3360_v2.jpg)

  With the sensor pins firmly in place, secure them with tape so that they do not float. Solder 16 pins from the top side. Remove tape from the sensor and attach the lens from the top side.   
  ![cocot38mini_bg_](/images/bg_pmw3360_v2_2.jpg)

  Once you finish soldering, please confirm that mouse cursor moves when you move close to the sensor.

### Spring Pin Header

  In this buildguide spring pin headers are used as example, but you can follow the most steps when you use pin headers.

  Cut spring pin headers with a cutter knife and insert them into the top side of the sensor PCB as shown in the picture below. The picture shows 2x7pins and 1x6pins as example. Please make sure you insert them in the correct location.  
  ![cocot38mini_bg_](/images/bg_pga2040_1.jpg)

  ![cocot38mini_bg_](/images/bg_pinheader.jpg)

  Once you insert spring pin headers to the PCB, insert main PCB onto it. ***Pay close attention to the orientation of each PCB.***  
  ![cocot38mini_bg_](/images/bg_pinheader_2.jpg)

### Rotary Encoder (optional)

  If you prefer to using rotary encoder at the center of thumb clusters, insert a rotary encoder in the position shown in the picture and solder 5 pins from the bottom side.
  ![cocot38mini_bg_](/images/bg_rotary_encoder.jpg)


### Zirconia Balls

  Glue the zirconia balls to the 3D printed top case using a two-component epoxy glue.  
  ![cocot38mini_bg_](/images/bg_zirconia_1.jpg)

  Take a small amount of glue on the tip of a toothpick or similar tool and apply it to the three depressions on the top case.  
  ![cocot38mini_bg_](/images/bg_zirconia_2.jpg)

  Insert zirconia balls into the depressions with glue and leave them until they harden. If the glue overflows into the surrounding area, wipe it off before it hardens. After the zirconia balls are glued, it will look like the picture below.  
  ![cocot38mini_bg_](/images/bg_zirconia_3.jpg)


### Assembly

  After soldering, stack the top case on top of the PCB and put key switches from the corners. Pay attention not bend the pins of the key switches.  
  ![cocot38mini_bg_](/images/bg_assembly_1.jpg)

  ![cocot38mini_bg_](/images/bg_assembly_2.jpg)

  Fit the top case and the bottom case together. First, align the bottom case so that the grooves on the bottom side of it (1&2) engages with the top case.  
  ![cocot38mini_bg_](/images/bg_assembly_3.jpg)

  FIt the remaining grooves into the top case. Push in the order of 3>4>5 until they snap into the place. It will be easier to fit the bottom case into the top case if you push it while pulling the bottom case toward the far side.
  ![cocot38mini_bg_](/images/bg_assembly_4.jpg)

  Put rubber feet on the bottom case.
  ![cocot38mini_bg_](/images/bg_assembly_5.jpg)

  Put ball and keycaps, and take a photo.
  ![cocot38mini_bg_](/images/bg_assembly_6.jpg)


## Custom Keycodes

  Several custom key codes can be set for trackball operation.

  Keycode   |Description
  ---------|-----------
  `CPI_SW`  |Change the CPI of the trackball. With the default firmware, each press changes the CPI in the following order: 200 -> 400 -> 800 -> 1600 -> 3200 -> 200....
  `SCRL_SW` |Changes the sensitivity of the sensor in scroll mode. The higher the value, the smaller the amount of scrolling.
  `ROT_R15` |Turns the Y axis of the mouse sensor 15 degrees clockwise.
  `ROT_L15` |Rotate the Y axis of the mouse sensor 15 degrees counterclockwise.
  `SCRL_MO` |	Enables scroll mode for as long as it is pressed.
  `SCRL_TO` |Toggles between scroll mode and mouse mode each time it is pressed.
  `SCRL_IN` |Inverts the scroll direction.
  `AM_TOG` |Toggle the function of auto mouse layer.

  Custom key codes can be set in vial using the custom key code under the User tab.  
  ![CustomKeycode_rev](/images/bg_customkeycode.jpg)


## Notes
If you have any problems, please contact us at[Twitter](https://twitter.com/aki27kbd).

Also, it would be very encouraging if you could upload the completed photos to social networking sites. (If you don't feel comfortable uploading your photos, you can send them directly to us via DM.)

The hashtag is #cocot38mini .
