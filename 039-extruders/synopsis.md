## This video is about : 

What are extruders, what the extruder module is, how to configure and use it

## This video will teach the following things : 

* Introduction : Extruders are stepper motors that push filament, they are very similar to XYZ axes but do a different job
* Wiring : They are wired the same as XYZ steppers, typically on M4 for the first extruder and M5 for the second
* Show an example
* Configuration : You can create as many extruder modules as you want, however, each one of them will require an on-board stepper motor driver, or two free gpio pins to control an external driver
* You need to set the pins for that driver, either to M4 or M5 [show example], or to free gpio for an external driver
* If it's an on-board driver you also need to setup the current for it
* You also need to set the steps per mm [show how to figure that out]
* Testing : How to test your extruder, how to measure it's extruding the right length
* Troubleshooting : If it's not extruding the right distance, do a rule-of-three on the steps per mm 

## Links 

The description for this video should contain the following links : 

* http://smoothieware.org/extruder

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

