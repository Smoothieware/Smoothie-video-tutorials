## This video is about : 

Describe here what this video is about

## This video will teach the following things : 

* One thing
* Another thing

## Links 

The description for this video should contain the following links : 

* A link
* Another link

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

Authors note:  Monitor and control. Break down the difference between the two concepts and what role each one plays in automation. Separately and together. Tie this knowledge into input/output and GPIOs

In the world of automated machinery there are two types of automation capabilities. The ability to monitor and the ability to control.  Monitoring provides information about events or ongoing activity related to a task. And in order for monitoring to be effective it must be accurate. Some good examples of monitoring are temp location distance and even video falls into this category. The opposite of monitoring is control. Control is taking action based on an event or dictating action or movement based on activity. control allows you to manipulate temp, move to a location, or calculate distance etc.  it's also important to have very accurate control in response to monitored real-time events and activity. 

In order to do monitoring and control a connection is required to a hardware device via electrical wires or a circuit on a board. Each hardware device typically has a single connection to a control board that with a microcontroller.  Information flows in from the device or out to the device depend on the configuration. This information is transferred in the form of electrical signals. In addition there are specific connections that receive info and connections that send info. Receive connections are called INPUT and sending connections are called OUTPUT.  Most of the time the direction of information for the connection is handed by software and is configured ahead on time before the circuit is put into operation.  And in some cases the direction of information for connections cannot be changed based on the hardware design of the control board.  Any connection that accept INPUT/OUT is considered to be a General Purpose Input Output or GPIO.

So that is a general explanation, now lets look at the physical aspects of a GPIO and how they are implemented on most control boards.  Below is picture of a 32-bit MCU that has been soldered on to a PCB board.

{LPC_100.JPG}

The MCU is very tiny and surrounded by 100 pins that allow for connecting other devices as well as power.  These pins are physical connections that make GPIO possible.  As you can tell the MCU pins are very close together on all sides so connections to other devices must be spread out over the control board.  These pins are also solder to connections that lead out to larger pins which allow for wires to be connected that are typically part of another device.  

{LPC_100_TEXT.JPG}

## Authors

If you contribute to this video in any way, please add your name to this list : 

* Mark Ingle

