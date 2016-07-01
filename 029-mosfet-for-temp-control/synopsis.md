## This video is about : 

Using a mosfet output and a thermistor input to control the temperature of a heating element

## This video will teach the following things : 

* You need to know what is a mosfet and how to power it ( from the basic mosfet video )
* Intro : Temperaturecontrol is a module, you can create as many as you want just by adding them to the config file, each module needs a mosfet to control a heater, and a thermistor to read temperature
* You use gcodes to tell the module what to do, and it maintains temperature by turning the heater on and off based on the temperature the heater reads
* Input : Explain what is a thermistor ( it's resistance changes based on it's temperature, different types change differently so we need to tell smoothie what type it is )
* There is a special type of input ( thermistor input ) on Smoothieboards named T1, T2, etc ... [show]
* You wire the thermistor to the thermistor input [show]
* Output : You must choose a mosfet that is adequate for your load ( fan, hotend, bed ), based on current
* Make sure the wiring is good : good contact, no shorts ( dangerous )
* Make sure the mosfets are getting power and the current is adequate ( see mosfet power input video )
* Configuration : enabling the module
* Telling Smoothie what thermistor you are using, and on what port it is connected
* Telling Smoothie on what mosfet the heater is connected
* Testing : Using M105 to check if the thermistor is reading temps correctly
* Set temperature low, check if it rises and if it stops rising, if it doesn't stop everything immediately and debug [show, both good and bad cases]
* Set temperature high, see if everything goes well [show]
* Difference between bang-bang and PID, and the fact there is a video on PID
* Usage : How to control via gcode
* Troubleshooting : What to do if it doesn't work
* You must absolutely watch the video on temperaturecontrol safety

## Links 

The description for this video should contain the following links : 

* http://smoothieware.org/temperaturecontrol

Also add any other information that should be added

## Video plan

The video is composed of the following sections : 

* Introduction
* Wiring ( Input and Output )
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

