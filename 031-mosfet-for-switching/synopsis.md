## This video is about : 

This video is about using the switch module to control a simple load ( like a fan ) via Gcode.

## This video will teach the following things : 

* To watch this video you must have watched the gpio and power supply videos 
* You need to know what is a mosfet and how to power it ( from the basic mosfet video )
* Switch is a general purpose module for mapping gcodes and inputs. You can configure as many as you want. You can cause a gcode to control an output, cause an input to trigger a gcode, or even cause an input to control an output. Here we will study how to configure a gcode to control a fan.
* You use gcodes to tell the module what to do, and it turns the fan on or off by using a pin to control the mosfet
* Output : You must choose a mosfet that is adequate for your load ( fan, hotend, bed ), based on current
* Make sure the wiring is good : good contact, no shorts ( dangerous )
* Fans require you have a diode across the output or the fan can burn the mosfet. Some v2 boards have it on-board, others require you add it yourself in your wiring.
* Make sure the mosfets are getting power and the current is adequate ( see mosfet power input video )
* Configuration : enabling the module
* Telling Smoothie what gcode turn the module on and off
* Telling Smoothie on what mosfet the load is connected
* Testing and usage: Using gcode to control the load
* Troubleshooting : What to do if it doesn't work

## Links 

The description for this video should contain the following links : 

* http://smoothieware.org/switch

Also add any other information that should be added

## Video plan

The video is composed of the following sections : 

* Introduction
* Wiring
* Configuration
* Testing
* Usage
* Troubleshooting

## Assets

Assets are pictures and videos to be displayed in the video.
Please here list and describe the various assets. They should be commited to github in this folder.

* One asset
* Another asset

## Video synopsis

Here add the text for this specific video

## Authors

If you contribute to this video in any way, please add your name to this list : 

* Arthur Wolf

