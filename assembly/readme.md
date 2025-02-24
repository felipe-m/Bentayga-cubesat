# Assembly instructions

Before assembling the cubesat, have all the electronics connected and make sure that they work. Disconnect the batteries and electronics before the assembly. 

Check the CAD files, and get all the 3D pieces printed and the plates milled.

Get all the components of the [BOM](./../bom_bentayga_cubesat.ods)
Have pliers, Allen keys, screwdrivers, small zip ties, .... Silicone would be very useful to place the t-slot nuts and prevent them from sliding.

The cubesat has 6 faces, they will be named according to this reference:

![References](../imgs/cubesat_full_orto_names.jpg)

---

## Warning

Take into account that once you close the profiles, you cannot place square bolts and in many times even nuts.

The following picture shows that you cannot add any nut or bolt in the blue profile. In the inner slot of the green profile you can add nuts, but not bolts.

Therefore, before closing a profile think if all the nuts and bolts are placed, and what are you going to attach to the profile.

![nut_warning](./imgs/cad/00_warning.png)

It is recommended to read all the instructions once before starting the assembly because there are some information that it is useful to know beforehand.

---

## Place nuts in 80mm-profiles

There are eight 80mm-profiles at the two squared faces of the cubesat (four at each face). The figure shows one of this faces.

![nuts 8mm](./imgs/cad/01_nuts_80mm_profiles.png)

All these profiles have 3 sliding nuts in one side and 2 in the other (you could put 4 but it is not necessary). These nut holes are marked in turquoise circles in the figure. The red circles indicate that these nuts are optional.

Place 2 and 3 sliding nuts in two consecutive sides of these eight profiles.

We recommend that you align these nuts with the holes of the plates and put some silicone to prevent the nuts from sliding. So they are easier to screw with the bolts.
It is not necessary to be super exact, since the silicone leaves room for moving the nuts a little bit. You don't need to wait until the silicone is dry.

The following pictures shows the process.

![nuts 8mm](./imgs/pic/01_nuts_80mm_profiles.jpg)

![nuts 8mm](./imgs/pic/01_nuts_80mm_profiles_b.jpg)

---

## Assemble the Down panel

Now that you have nuts in the 80mm-profiles, we are going to assemble the Down plate.

The profile at the Cielo side has also a 3D part attached to it (see next figure).

Include two [M3 6-mm square headed bolts](https://www.makerbeam.com/makerbeam-square-headed-bolts-6mm-250p-for-makerbe.html).

Don't put silicone on these bolts

![nuts 8mm](./imgs/pic/02_bolt_sensors.jpg)

Put in the long 340.5mm profiles five sliding nuts, aligned to the plate holes. It is not necessary to put silicone in these nuts, but you could.

Now put the Down plate over the four profiles attached to it, and screw the M3 4mm Hexagon socket button head screws (ISO7380). Take care that the 80mm profiles have the nuts facing the correct side.

Place the long profiles to be symmetrical, leaving the same distance in each side.

![Down CAD](./imgs/cad/02_down_assembly.png)

The result should look like this

![Down picture](./imgs/pic/02_down.jpg)

---

## Attach the I2C hub to the Down plate

Use three M2 bolts around 6mm long. We have used one steel bolt and nut, and the other two plastic, but you can choose the material.

![I2C Hub cad](./imgs/cad/03_i2c_hub.png)

Picture from the bottom:

![I2C Hub cad](./imgs/pic/03_i2c_hub.jpg)

---

## Attach the Jetson Nano

First attach the Jetson Nano to its 3D printed support.

Then take two M3 square headed 6mm bolts and attach the lower part of the Jetson Nano support to it. Then put two M3 self locking nuts, tighten but not so much so you can still slide the Jetson Nano along the profile.

![Jetson CAD](./imgs/cad/04_jetson.png)

Picture from Top:

![Jetson picture](./imgs/pic/04_jetson.jpg)

---

## Attach the sensors support

First attach the four boards to the support with M2 plastic bolts and nuts.

-  MKR GPS Shield: connect to the ESLOV connector https://docs.arduino.cc/hardware/mkr-gps-shield
-  Grove - Temp&Humi&Barometer Sensor (BME280) https://www.seeedstudio.com/Grove-BME280-Environmental-Sensor-Temperature-Humidity-Barometer.html
- Two Grove - DS1307 RTC (Real Time Clock) for Arduino https://www.seeedstudio.com/Grove-RTC-DS1307.html

Attach the bottom of the support to the profile. There should be two 6mm square headed bolts in this profile, as indicated in the assembling of the Down panel.

Put the self locking nuts as in the Jetson Nano support, but not too tight to be able to slide the support later.


![Sensors CAD](./imgs/cad/05_sensors.png)

Picture from back:

![Sensors back picture](./imgs/pic/05_sensors_back.jpg)

Picture from Top:

![Sensors top picture](./imgs/pic/05_sensors_top.jpg)

---

## Attach the Arduino stack

Before attaching the support, **insert four sliding nuts in the profile**. They will be needed for the small camera support, and to contain the battery box.

Also insert two sliding nuts in the opposite profile (Right side) to contain the battery box.

First the Arduino stack should be mounted, also make sure that the components in the MKR MEM Shield have been soldered, and from this shield go the wires to the Jetson Nano and MOSFET for the heat pads (which is soldered in a different board).

The stack of Arduino boards is the following from bottom to top:

- MKR connector: https://docs.arduino.cc/hardware/mkr-connector-carrier
- MKR WAN 1310: https://docs.arduino.cc/hardware/mkr-wan-1310
- MKR MEM SHIELD: https://docs.arduino.cc/hardware/mkr-mem-shield
- MKR IMU SHIELD: https://docs.arduino.cc/hardware/mkr-imu-shield

Attach this stack to the 3D printed support and in the same way as the previous support, attach it to the profile with a 6mm M3 square headed bolt and a self locking nut. Do tighten the nut too much to allow sliding.

![Arduino CAD](./imgs/cad/06_arduino.png)

Picture from Top (the IMU shield was missing in the picture)

![Arduino top picture](./imgs/pic/06_arduino.jpg)

---

## Attach the multispectral camera

Using four 12-mm square headed bolts and self locking nuts, attach the multispectral camera at the Tierra side as shown in the figure:

![Multispectral camera CAD](./imgs/cad/07_multcamera.png)

---

## Insert the battery box

Just put it in place to check the dimensions

![Battery box CAD](./imgs/cad/08_battery.png)

---

## Attach the small camera support

Fist attach the original camera support to the 3D printed support, using two M3 6mm counter sunk bolts with self locking nuts.

Then use sliding nuts and tow hex button 4mm bolts to attach it to the profile. Do not tighten it to strong, so it can slide along the profile.


![Small camera CAD](./imgs/cad/09_smallcamera.png)

Notice how the original camera support is attached to the 3D printed support.


![Small camera picture](./imgs/pic/09_smallcamera.jpg)

---

## Attach the Cielo panel

Now that we have all the elements attached to the bottom, we are going to attach the Cielo panel.

First we have to attach the 80mm profile on Top. Make sure that it is oriented properly, with the 3 sliding nuts pointing to Cielo and 2 sliding nuts pointing to Top. Ideally, there would be silicone to prevent them from sliding.

![Cielo 1 CAD](./imgs/cad/10_cielo.png)


Picture of the first step to attach the Cielo panel. Notice the silicone on the side of the Cielo nuts to prevent the nuts from sliding.

![Cielo 1 picture](./imgs/pic/10_cielo.jpg)

Include the self locking M3 nuts, but don't tighten them too much yet.

Now position the sensors support on the exact position you want it (by sliding a little bit right or left), and tighten the self locking nuts at the bottom.

Now set the Cielo plate with the two vertical 80mm profiles. Using the M3 4mm-socket button bolts and the sliding nuts. Do not tighten them too much because you will probably need to adjust them.

For the adjustment, you may need to move the top 80mm profile, to center it. Once you have adjusted the bolts by placing in its position, take the plate out and adjust the top self locking nuts of the sensors support.

Once it is all set, put back the plate and tighten all the socket button bolts of the Cielo plate.

![Cielo 2 CAD](./imgs/cad/10_cielo2.png)

Picture with the plate before screwing the top and bottom socket button bolts

![Cielo 2 picture](./imgs/pic/10_cielo2.jpg)

---

## Set the antenna

The antenna can be placed outside over the Down plate, there is a hole for the cable, and some holes  that can be used to hold it with zip ties. However, since it can protrude more than what is allowed, we have decided to put it inside, between the Jetson Nano 3D support and the Right plate.

The [antenna](https://store.arduino.cc/products/dipole-pentaband-waterproof-antenna) has an adhesive tape, nevertheless it is recommended to attach it with a zip tie, as shown in the next picture.


![Antenna picture](./imgs/pic/11_antenna.jpg)

---

## Secure the battery box

The battery box has holes on top to secure it, but in addition, you can include one or two [right angle brackets](https://www.makerbeam.com/makerbeam-right-angle-brackets-12p.html) to hold it.
In case you put two, put them at each side.


![Battery stop](./imgs/pic/12_battery_stop.jpg)

---

## Attach the Tierra panel

In a similar way to the Cielo panel, put the Tierra panel.

This panel is easier because it has not any support board attached, therefore you can mount the panel with the three 80mm profiles (Left, Top and Right) and attach it to the bottom 80mm profile.

![Tierra panel 1](./imgs/pic/13_tierra_1.jpg)

![Tierra panel 2](./imgs/pic/13_tierra_2.jpg)

---

## Assemble the Top-Right 340.5mm profile

Insert two M3 6mm square headed bolts and tow M3 12mm square headed bolts to attach the top of the Jetson Nano support and the top-right side of the camera, respectively.

![Top-right profile](./imgs/pic/14_top_right_1.jpg)

Put the profile in its place, passing the bolts through the camera support:

![Top-right profile 2](./imgs/pic/14_top_right_2.jpg)

And the Jetson Nano support:

![Top-right profile 3](./imgs/pic/14_top_right_3.jpg)

Before tightening the bolts with self locking nuts, make sure that the Top profile is aligned with the bottom, and it is placed symmetrically, i.e. it has the same protrusion length in the Tierra direction  as in the Cielo direction.

Put the right plate on top to check if it is aligned. If it is aligned, tighten all the nuts.

Check if the sliding nuts inside the vertical 80mm profiles are aligned with the holes (thanks to the silicone), correct their position if they are not aligned.

---

## Assemble the Right panel

Put 10 sliding nuts with their M3 4mm socket button head bolts in the Right panel as shown in the picture. There are more holes that you can use, but with these is enough.

Leave the nuts loose, just enough to keep them with the bolt.


![Right panel 1](./imgs/pic/15_right_panel_1.jpg)

From one end, introduce the nuts in the profile slot and slide the panel until it is centered.

![Right panel closing](./imgs/pic/15_right_panel_closing.jpg)

Tighten all the bolts of the right panel:

![Right panel closed](./imgs/pic/15_right_panel_closed.jpg)

---

## Adjust battery box

Adjust all elements inside, making sure that there is room for everything, and attach it to the profile with three M3 4mm socket button head bolts and sliding nuts.

![Battery box bolt](./imgs/pic/16_battery_box_1.jpg)

The sliding nuts can be introduced from one end, and pushed until they are aligned with the battery box holes.

![Battery box bolt](./imgs/pic/16_battery_box_2.jpg)

---

## Assemble the Top-Left 340.5mm profile

This is similar to the Top-Right profile.

Using two M3 6mm square headed bolts and tow M3 12mm square headed bolts to attach the top of the Jetson Nano support and the top-right side of the camera, respectively.

Alternatively, as shown in the picture, you can use sliding nuts and blots.

Do the same as in the Top-Right, making sure everything is aligned. Superimpose the plate to check the alignment.


![Top-left profile](./imgs/pic/17_top_left.jpg)

Once it is aligned, tighten the bolts, and also secure this side of the battery box, as it was done before on the right side.

---


## Fix the switches and MOSFET board

Place the [switches 3D printed support](../cad/stl/switch_support.stl) and the MOSFET board on the Top-Left profile, using sliding nuts and M3 4mm socket button head bolts.
Check that the switches are aligned with the plate holes.


![Switchs and MOSFET board](./imgs/pic/18_switch.jpg)

![Switchs and MOSFET board 2](./imgs/pic/18_switch_2.jpg)

---
## Assemble the Left panel

Do the same as in the right panel.
We have included two additional bolts, for the holes near the camera and switches.

![Left panel 1](./imgs/pic/19_left_panel_1.jpg)

![Left panel 2](./imgs/pic/19_left_panel_2.jpg)

Tighten the bolts and place the small camera:

![Left panel 3](./imgs/pic/19_left_panel_3.jpg)
