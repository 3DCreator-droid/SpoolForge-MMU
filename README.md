# SpoolForge MMU - A budget friendly DIY AMS
As of right now, this is no different than the repo it was forked from, so go there instead! I have limited time, so I can't update this a bunch, but it will happen eventually. My recomendation

Update Roadmap:

-Ease of use macros (the original creator has done a great job already, but there are a few things I would like to add)

-AMS.cfg generator: Similar to the 3Dchameleon code generator, but instead of generating button presses, it will generate your macros.

-SpoolForge Enclosure 

-2 new toolheads (bowden and direct drive) for printers with the Ender-3 extuder plate (encluding CR-10, E3v2, E3 pro, and maybe E3 max)
  
  Bowden Toolhead: CinderLance
 
  Direct Drive: EmberCore 

  (chatgpt generated "SpoolForge" themed names haha)

-More detailed instructions

-Mainsail theme

More updates coming soon!

## Current BOM (may change)
-A Klipper printer with a spare USB port and a filament cutter (the cutter technically isn't required, but you will probably die trying to perfect tip shaping)

-CNC Shield v3 Kit (you could use other boards, like a BTT pico, but this is the most cost effective):
  https://www.aliexpress.us/item/3256808331843303.html?spm=a2g0o.productlist.main.25.78478171IR3BQ9&algo_pvid=1e7f1e16-7855-4b98-9219-3707b2227be7&algo_exp_id=1e7f1e16-7855-4b98-9219-3707b2227be7-12&pdp_ext_f=%7B%22order%22%3A%221%22%2C%22eval%22%3A%221%22%7D&pdp_npi=4%40dis%21USD%2111.08%217.87%21%21%2111.08%217.87%21%402103246617450025792606825e5068%2112000045525251744%21sea%21US%216325345170%21X&curPageLogUid=845Ioq7nRSY0&utparam-url=scene%3Asearch%7Cquery_from%3A
  
-2-4 Nema 17 stepper motors (the amount of motors is the amount of colors. Pancake steppers worked for me, but I had quite a few torque-related issues)

-2-4 Extruders:
      A quick note: there are tons of options for extruders. You could go with the cheap Mk8, or go with the quite strong Voron M4. You could even get a mix of them, but that would       require some manual configuaration. This is up to you. The extruder options are listed below.

  Aluminum Mk8:
https://www.aliexpress.us/item/3256806663498456.html?spm=a2g0o.productlist.main.7.3993PA2DPA2DZq&aem_p4p_detail=202504181147474377157000056890004338616&algo_pvid=00f76bf7-6841-48a0-a042-3cc0785fac9a&algo_exp_id=00f76bf7-6841-48a0-a042-3cc0785fac9a-3&pdp_ext_f=%7B%22order%22%3A%22201%22%2C%22eval%22%3A%221%22%7D&pdp_npi=4%40dis%21USD%214.84%214.84%21%21%2135.15%2135.15%21%402101e7f617450020674765210e4072%2112000038509805535%21sea%21US%216325345170%21X&curPageLogUid=QauW0djtvX1A&utparam-url=scene%3Asearch%7Cquery_from%3A&search_p4p_id=202504181147474377157000056890004338616_1

   Dual Drive Mk8:
https://www.aliexpress.us/item/3256807474433787.html?spm=a2g0o.productlist.main.7.7bdb44f0L5hHoR&aem_p4p_detail=202504181149537771076731941640004421295&algo_pvid=2f486567-52fc-4f1f-b45a-fb817e7d36e5&algo_exp_id=2f486567-52fc-4f1f-b45a-fb817e7d36e5-3&pdp_ext_f=%7B%22order%22%3A%22123%22%2C%22eval%22%3A%221%22%7D&pdp_npi=4%40dis%21USD%215.51%215.51%21%21%2140.01%2140.01%21%402101c5b117450021933307538e8081%2112000041695695206%21sea%21US%216325345170%21X&curPageLogUid=nPevx7GM6SZT&utparam-url=scene%3Asearch%7Cquery_from%3A&search_p4p_id=202504181149537771076731941640004421295_3

  Voron M4 (note: this requires a soldering iron and parts printed in ABS/PETG to assemble):
https://www.aliexpress.us/item/3256804563706032.html?spm=a2g0o.productlist.main.1.8ad49458dXoKdq&algo_pvid=55409829-aba2-4b2c-98e2-fa23fc7f94cb&algo_exp_id=55409829-aba2-4b2c-98e2-fa23fc7f94cb-0&pdp_ext_f=%7B%22order%22%3A%22128%22%2C%22eval%22%3A%221%22%7D&pdp_npi=4%40dis%21USD%216.09%216.09%21%21%216.09%216.09%21%40210337c117450022781751039efcc7%2112000033727809094%21sea%21US%216325345170%21X&curPageLogUid=nkyuJlWQJAKZ&utparam-url=scene%3Asearch%7Cquery_from%3A

  BMG Clone:
https://www.aliexpress.us/item/3256806582539101.html?spm=a2g0o.productlist.main.5.3993PA2DPA2DZq&algo_pvid=00f76bf7-6841-48a0-a042-3cc0785fac9a&algo_exp_id=00f76bf7-6841-48a0-a042-3cc0785fac9a-2&pdp_ext_f=%7B%22order%22%3A%22217%22%2C%22eval%22%3A%221%22%7D&pdp_npi=4%40dis%21USD%215.15%215.15%21%21%215.15%215.15%21%402101e7f617450020674765210e4072%2112000038237815138%21sea%21US%216325345170%21X&curPageLogUid=Ys3xBXr3C8cF&utparam-url=scene%3Asearch%7Cquery_from%3A

-USB-B cable:
https://www.aliexpress.us/item/2251832513860879.html?spm=a2g0o.productlist.main.1.687418f41yWhw3&algo_pvid=df7df7bc-42b9-4d71-893d-0d1a78601844&algo_exp_id=df7df7bc-42b9-4d71-893d-0d1a78601844-0&pdp_ext_f=%7B%22order%22%3A%222890%22%2C%22eval%22%3A%221%22%7D&pdp_npi=4%40dis%21USD%211.65%211.65%21%21%211.65%211.65%21%402103244817450028168368289e6112%2112000018606724058%21sea%21US%216325345170%21X&curPageLogUid=jOroO8Y2KVxR&utparam-url=scene%3Asearch%7Cquery_from%3A

-12v power supply:
https://www.aliexpress.us/item/3256802164880804.html?spm=a2g0o.productlist.main.47.34ebb93e8Rlgdy&aem_p4p_detail=202504181203262467060604996880000736786&algo_pvid=1e8afa5a-ff71-4802-9519-3941d4019055&algo_exp_id=1e8afa5a-ff71-4802-9519-3941d4019055-23&pdp_ext_f=%7B%22order%22%3A%22154%22%2C%22eval%22%3A%221%22%7D&pdp_npi=4%40dis%21USD%216.84%214.79%21%21%216.84%214.79%21%402101e9a217450030061207261ecf14%2112000020516705499%21sea%21US%216325345170%21X&curPageLogUid=VpcMQrmkfKrB&utparam-url=scene%3Asearch%7Cquery_from%3A&search_p4p_id=202504181203262467060604996880000736786_6

-PTFE Tube Bundle:

-4 way PTFE splitter (you could print one, but these are better):
https://www.aliexpress.us/item/3256807550249750.html?spm=a2g0o.productlist.main.1.684d213f3RH6YR&algo_pvid=c69ea115-564a-436d-bf3e-ed493b363d01&algo_exp_id=c69ea115-564a-436d-bf3e-ed493b363d01-0&pdp_ext_f=%7B%22order%22%3A%221405%22%2C%22eval%22%3A%221%22%7D&pdp_npi=4%40dis%21USD%216.26%216.26%21%21%2145.46%2145.46%21%402101c72a17450033201354999ec059%2112000042035346114%21sea%21US%216325345170%21X&curPageLogUid=8JMmaVY9ySk8&utparam-url=scene%3Asearch%7Cquery_from%3A

-Bowden Connectors:
https://www.aliexpress.us/item/3256802572907275.html?spm=a2g0o.productlist.main.57.55986B5e6B5eSq&algo_pvid=23faf04c-f69c-4df6-9402-d2a52fad253c&algo_exp_id=23faf04c-f69c-4df6-9402-d2a52fad253c-28&pdp_ext_f=%7B%22order%22%3A%22196%22%2C%22eval%22%3A%221%22%7D&pdp_npi=4%40dis%21USD%213.10%213.10%21%21%213.10%213.10%21%402101c59517450035053373658e09e1%2112000022053061980%21sea%21US%216325345170%21X&curPageLogUid=q6LMgA1zrk4y&utparam-url=scene%3Asearch%7Cquery_from%3A

-Bowden Tubes (get the 2 or 4 meter option so you have leftover):
https://www.aliexpress.us/item/3256806056618135.html?spm=a2g0o.productlist.main.1.356bMlGSMlGS68&algo_pvid=7f62b59f-9fd6-46db-8c4e-8943464b8aa7&algo_exp_id=7f62b59f-9fd6-46db-8c4e-8943464b8aa7-0&pdp_ext_f=%7B%22order%22%3A%226160%22%2C%22eval%22%3A%221%22%7D&pdp_npi=4%40dis%21USD%211.30%211.30%21%21%211.30%211.30%21%402101d9ef17450036329265114e5bc0%2112000038262545100%21sea%21US%216325345170%21X&curPageLogUid=M8doN481EznU&utparam-url=scene%3Asearch%7Cquery_from%3A

-Pin Jumpers (for allowing the "A" axis driver to connect to a motor, and to allow microstepping):
https://www.aliexpress.us/item/2255800354403384.html?spm=a2g0o.productlist.main.3.2f56f8N4f8N4LT&algo_pvid=f1ef94a7-c302-485d-89c2-8fd11aad9158&algo_exp_id=f1ef94a7-c302-485d-89c2-8fd11aad9158-1&pdp_ext_f=%7B%22order%22%3A%22751%22%2C%22eval%22%3A%221%22%7D&pdp_npi=4%40dis%21USD%210.88%210.88%21%21%210.88%210.88%21%402103244b17450398423115594ea683%2110000002790230890%21sea%21US%216325345170%21X&curPageLogUid=9QTb5Fm6GIvW&utparam-url=scene%3Asearch%7Cquery_from%3A

-A way to hold the spools while printing

[end of updated instructions]

## Arduino Steps
- Attach Arduino to CB1/Raspberrypi
- Flash Arduino
- Upload multi_color.cfg to your klipper machine
  - Update MCU Serial path
- Setup up your Arduino and CNC sheild to your needs

## Flashing the Arduino
The hardest part of this project, other than tuning the steppers, will be flashing the arduino.
Depending on what version of debian you are running this might require you to add some specific libraries to your computer running klipper.

See this if you have any issues with the flashing procedure:
[https://github.com/Klipper3d/klipper/issues/4938#issuecomment-1094246978](https://github.com/Klipper3d/klipper/issues/4938#issuecomment-1094246978)

If you are using KIAUH to manage your klipper install you can build and flash right from inside of KIUAH

Open up KIAUH and select the following:
- [ADVANCED]
- [BUILD + FLASH]
- Select the configuration options below

### Options to select for Arduino Uno
```
Enable extra low level configuration options
MCU Architecture: Atmega AVR
Processor model: atmega328p
Processor speed: 16 MHz
Baud rate for serial port: 250000 
```

### Troubles flashing arduino??
[https://github.com/Klipper3d/klipper/issues/4938#issuecomment-1094246978](https://github.com/Klipper3d/klipper/issues/4938#issuecomment-1094246978)



# Preparing the slicer!

There are a few custom Klipper Macros to make some of this easier.
- UNLOAD_COLOR
- LOAD_COLOR
- CHANGE_COLOR
- SET_COLOR

The filament changing macros currently don't have a set of temps to allow the change so you'll need to heat your extruder before using them.

Our change gcode was put together in Orca Slicer so you will need to adjust depending on your slicer. In your filament change gcode you'll want to set it to something similar to the following:
```
; For Orca Slicer
; - Custom AMS tool T{next_extruder} -
CHANGE_COLOR NEXT_COLOR={next_extruder} DISTANCE=200
M117 Custom AMS Tool T{next_extruder}
```

## Activating Multi-Color
add ``[include 'multi_color.cfg']`` to you printer.cfg file.

## Extruders in tandum vs separate
Depending on your needs one way may benefit you more than another.

- Tandum -> Passing material to a main extruder, best for direct drive extruders
- Separate -> Passing material straight from auxillery extruders to hot end, best for bowden setups

Reguardless of your method you will want to check and update the rotation distance of the auxillery extruders you are using.

### Tandum Operation
When hooking up your multi extruder for tandum you will be passing from the PTFE extruder into your main extruder. 

### Separate Operation
This config utilizes the SYNC_EXTRUDER_MOTION klipper macro to control the extruders on and off. If you want to directly extruder from your auxillery steppers and not use the built in extruder for your machine uncomment the line:

```
# SYNC_EXTRUDER_MOTION EXTRUDER="extruder" MOTION_QUEUE=''
```

This will deactive your main extruder and let the other extruders take main control.

You'll then need to go from your PTFE Joiner straight into the hotend.

#### Note:
In Orca turn off ramming when running separate. Orca slicer does set ramming properties with a PRESSURE_ADVANCE setting for klipper machines that I haven't figured out how to get rid of. If you removed the main extruder from the motion queue this does throw an error and will stop your print dead in it tracks. WHen the main extruder is removed it has no idea what extruder to apply the pressure advance to.

# Want to contribute?!
Happy to have any help! I am not yet the best will all of the amazing things you can do with klipper, but any other ideas of things we can add or improve with this are greatly appriciated!

Open a issue or possibly a pull request and we can have some fun troubleshooting!

