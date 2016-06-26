## This video is about : 

How to determine the power requirements and power limits, to choose your power supply and decide how to wire things.

## This video will teach the following things : 

* What is voltage, what is current, what is power
* How do you do the math to figure one out by having the other two
* What are power inputs and outputs
* How to determine power requirements
* How to determine power limits ( connectors, cables )
* How to decide how to wire things
* A simple example for a basic 3D printing setup, to put what we learned into application

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

Now that you are able to configure the board, and communicate with it, it is time to provide power to it so that it can do things.

Your Smoothieboard has power inputs, and power outputs.

The firmware can control whether some of the outputs are active or inactive, thanks to components called “Mosfets”.

For an output to be able to provide power to whatever is connected to it, the corresponding input must be getting power.

So it goes like this : Your PSU provides electricity to an input on the Smoothieboard, that electricity enters the Mosfet, then the firmware chooses whether the Mosfet lets the electricity out or not. If the electricity is let out, it goes to the output, and then to whatever is connected to that output, for example a heating element or a fan.
Power input

Smoothie has two types of mosfets : small ones that are capable of running fans or hotends, and big ones that are capable on running beds or hotends. {show}

Let’s go over how to power each mosfet one by one.

The first two large mosfets share a common power input
If you want to use the first large mosfet output {show}, you need to provide power to this input {show}.
{show assembly with PSU connected to input, lamp connected to output, blinking}
If you want to use the second large mosfet output {show}, you need to provide power to this input {show}.
{show assembly with PSU connected to input, lamp connected to output, blinking}

The first two small mosfets share a common power input.
If you want to use the first small mosfet output {show}, you need to provide power to this input {show}.
{show assembly with PSU connected to input, lamp connected to output, blinking}
If you want to use the second small mosfet output {show}, you need to provide power to this input {show}.
{show assembly with PSU connected to input, lamp connected to output, blinking}

The last two mosfet, one big, one small, get their power from the VBB ( stepper motor ) input.
If you want to use the third large mosfet output {show}, you need to provide power to this input {show}.
{show assembly with PSU connected to input, lamp connected to output, blinking}
If you want to use the third small mosfet output {show}, you need to provide power to this input {show}.
{show assembly with PSU connected to input, lamp connected to output, blinking}

Mosfets are not the only thing you can control on the board : you can also control stepper motors. Those stepper motors receive their power via the VBB connector {show}.

### Current limits

Your board can not control an infinite amount of power, it has limitations.


## Authors

If you contribute to this video in any way, please add your name to this list : 

* Arthur Wolf

