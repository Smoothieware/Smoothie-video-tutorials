## This video is about : 

How to get 5V into the Smoothieboard so that the microcontroller does things.

## This video will teach the following things : 

* What is the logic power for ( microcontroller, peripherals )
* Difference between logic power and main power
* How to provide logic power to the board ( USB, Vreg, ext. input ) 
* How to troubleshoot logic power problems

## Links 

The description for this video should contain the following links : 

* A link
* Another link

Also add any other information that should be added

## Video plan

The video is composed of the following sections : 

* Introduction
* Troubleshooting

## Assets

Assets are pictures and videos to be displayed in the video.
Please here list and describe the various assets. They should be commited to github in this folder.

* One asset
* Another asset

## Video synopsis

The microcontroller on the board, executes the firmware. To do so, it requires electrical power.

To move the motors you connect a 12 or 24v power supply ( VBB ) to the board. You could think that that is what will also power the microcontroller, but it isn’t so.

The microcontroller requires 5V power, and therefore, is going to need another source of power ( 12 or 24v being much too high ).

There are different ways to provide 5V power to the board.

For example, you can plug a USB cable into the Smoothieboard, and into your computer. When you do so, the computer will be providing 5V power to the board  {demonstrate board turning on}, and the microcontroller will be able to execute the firmware and control it’s peripherals.

But there are situations in which you do not want to have a USB cable connected. 
USB cables can be subject to much more problems than other means of controlling the board, and in some situations, will disconnect.

If you do not want to use a USB cable, for example because you are using Ethernet, or a control Panel, then you need an alternative way of providing the 5V power to the board. 

One way to do this, is to provide 5V power via the 5V power input {show}. This is a good option for example if your power supply has an available 5V output. 

Another way is to install the voltage regulator on your board. This will take the 12 or 24v power provided to the stepper motors, and convert it to 5V. [http://smoothieware.org/voltageregulator]. It requires soldering the component {show}.

These are the three ways to power your microcontroller. Once it is powered, you can start configuring and talking to it.

### Troubleshooting

There is a series of 6 LEDs near the microcontroller {show}.

The red one turns on if VBB ( motor power ) is supplied.

The orange one turns on if the microcontroller is getting 3.3v power ( the 5V power is converted to 3.3v before getting to the microcontroller ).

The 4 green LEDs indicate the status of the working microcontroller.

If the Orange LED is not turning on, you are not providing power to the microcontroller.

## Authors

If you contribute to this video in any way, please add your name to this list : 

* Arthur Wolf

