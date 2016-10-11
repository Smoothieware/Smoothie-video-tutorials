## This video is about : 

In this video we learn what endstops are, and what we can use them for in Smoothie ( homing, and limit switches )

## This video will teach the following things : 

* An endstop is a mechanical switch that is put at an end of a given axis so we can detect when we are getting close to an end of a given axis
* Homing is telling Smoothie to go "seek" an endstop for an axis ( or all of them ). Once it is hit, we know where we are, before we didn't
* Limit switches is just using those same endstops to prevent the user from going out of bounds
* There are 6 endstop inputs : Two for each of the three axes.
* It is constituted of + and -, and a signal line ( that is read by Smoothie )
* Explain what is NC and NO, and what are pullups and pulldowns.
* Explain how to wire a NC endstop ( classical case )
* Explain how to wire "powered" endstops, like hall-effect and optical
* How to configure homing in the config file ( for a cartesian, simplest case )
* Testing your endstops ( M119 )
* Using the G28 command
* Enabling and testing limit switches ( demonstrate )
* Troubleshooting : use M119 to test, if false positives : use debounce, if stuck in place : reduce speeds

## Links 

The description for this video should contain the following links : 

* http://smoothieware.org/endstops

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

In order to implement position control for most automated systems there has to be a way to determine “the current position” of the object that is being controlled.  These physical limits can be the end of a rail, the edge of a table or wall.The first step in controlling position is to virtualize the actual physical limits and boundaries.  Depending on the process or application there are many ways to do this.  Most of the time to define boundaries a piece of hardware is used called an Endstop.  And it does exactly what it is called……”You are at the end…STOP!!”  Usually an endstop has a sensor of some kind that is “triggered” by physical touch or proximity of a moving object.  Depending on the requirement the object may stop, bounce back into place, or move in the other direction which may also have an endstop waiting to be triggered.  The endstop itself is nothing more than a relay switch anchored down tightly.  But it serves a very important function.  Before any type of position control can take place the control software must have awareness of physical limits to carry out a task.

From a logical perspective an endstop provides a means to define coordinates of an axis simply by knowing the starting point (or ending point) for the axis.  Once the starting location is physically determine it can be used as reference for movements along the axis.  The distance the object travels on the axis can be limited by software or another endstop.  Having the starting and end points defined then makes it easy to control the object up, down, left, and right with certainty and accuracy.  Endstops are so important that they are “touched” each time a job is ran on automated systems.

There is also an assumption that all things remain constant for the logical control to work every time.  If the controller thinks that 150 ticks will move the object three inches it's important that there isn’t any slips or hang during the movement.


## Authors

If you contribute to this video in any way, please add your name to this list : 

* Arthur Wolf
* Mark Ingle
