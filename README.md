# Greecher Voron 0.2 R1 LDO Kit, V0.2951 registered 8/9/2023

This is the Klipper Config for my Voron 0.2 . This is built out with everything I wanted to do, may add mods later, but as of now completely happy with it.

## About this repo

This is the real actual config that I run on my printer. This is the repository that is created from a push from my printer to share, but also backup in case of catastrophe.  For the use cases of this printer and mods deployed, maybe of use to someone else whom has those mods. ***Use at your own risk.***

## Goals for this printer
* A printer that would act as a backup to my V2.4R2.
* A printer that gets used more for experimental purposes and exotic materials. I commonly print in ASA now, but want to try out PC-CF and more.  I design most of what I consume, but occasionally will visit [Printables](https://www.printables.com), as well as share out my own designs there as well.
* Usability, Speed & Print Quality - I want to test the bounds of speed and still maintain quality.

## About the Printer's Hardware

This is a Voron V0.2 R1 LDO kit built in mid 2023.  I actually sourced my own printed parts from my Voron V2.4R2 inASA material.  LDO was kind enought to have pre done print plates, so was easy enough to get the correct printed parts the first time. 

Here is a list of the final build & mods.

* Mini Stealthburner with CW2 Toolhead - note the LDO kit comes with the latest pancake extruder motor as well as Bondtech gears.
* E3d Voron Revo - also a kit included item.
* Nevermore chamber filter.  This works well on keeping my chamber temperatures constant and odor free, regulary at 50C after 20 minutes preheat for my ASA prints, and even 55C after 1 hour.
* SKR Pico mainboard & Raspberry Pi 4 Model B & LDO Picobilical setup.
* Crowsnest to a Logitech C920X webcam.
* A usb plugable adxl module driven by it's own raspberry pi pico, this is from [Nero's Youtube](https://www.youtube.com/watch?v=W_VHbT_tsZw&ab_channel=NERO3D).
* Added the included filament sensor but on a Mod back plate instead of through the wiring guts.
* Added a Matchstick set of chamber lights
* Made a Keystone to pass throught Ethernet, HDMI & USB for the rear skirt, this is my own designed modification.
* Made various changes to properly get my print_start better, and working properly with prusaslicer start gcode. This version ensures to make bed heat to final temp at the start, extruder to start @ 150C for TAP max temp, then do the calibrate, then properly set and ensure the extruder and bed temps before proceeding.

## Klipper Software Customization
* Sensorless X & Y homing, this [guide](https://docs.vorondesign.com/community/howto/clee/sensorless_xy_homing.html) made it a snap, and works excellently.

## Overall Experience
* The build was pretty flawless, but it is back to the old a bit with a spring loaded manual leveled bed.  I did get 2 steel bed sheets from Fabreeko (a fine company), but the sheets where some .5mm difference, so managing the correct Z offset has been challenging.
* The Discord server for VORON has sooo many helpful hints and people, use it whenever you get stuck!
* One minor, I had a heck of a time fitting the picobilical cable, as it was extremely tight.  Luckily I had a board from my other LDO kit with the same connector.  Multipe insertions and it was working smooth enough to install.  Been solid so far.

