## This video is about : 

How to determine the power requirements and power limits, to choose your power supply and decide how to wire things.

## This video will teach the following things : 

* What is voltage, what is current, what is power
* (TODO) What are AC and DC power. Mains power can kill you, DC power can hurt you. Ask an adult for help
* (TODO) Always unplug mains before doing any kind of mains-related wiring. Do not leave mains exposed.
* (TODO) How to provide mains power to your PSU
* How do you do the math to figure one out by having the other two
* What are power inputs and outputs
* How to determine power requirements
* How to determine power limits ( connector ratings, cable diameter )
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
* Safety concerns
* Determining if your PSU is enough or you need two
* Identifying the poles
* Connecting 3 wires and preventing shorts
* Adding a fused on/off switch
* Connecting fans, LEDs that are 'always on', adding switches as desired
* Connecting the Smoothie to the PSU
* Understanding the distribution of power between the PSU and the USB connection
* Troubleshooting

## Assets

Assets are pictures and videos to be displayed in the video.
Please here list and describe the various assets. They should be commited to github in this folder.

* Sample, common (LED) PSU image
* 'Brick' type PSU image used on laptops
* ATX type PSU image
* Volt/Ammeter
* Examples of fused and lit switches
* Examples of cases/enclosures for PSUs

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

-Show clearly the location and description of poles on the various PSU types (animation to show current flow?).  Contrast where the input plug is wired (where applicable), what the output wires look like
-Discuss safety -- no shorts, consider wearing rubber gloves initially, make absolutely sure + is + and - is -.  
-Show how to put an ATX PSU into service (differs from other types) -- e.g. using an aftermarket 20/24 pin plug and switch, or using a patch wire to short the 'green wires'
-Calculate Watts: how much power is at each terminal (Volts and Amps).  Determine voltage at outputs (easy to do with LED and ATX PSUs, a bit fiddly with 'bricks'
-Calculate power required for each part of the printer: motors, board, heatbed(s), hot end(s), fans, LEDs.  Compare to PSU output.  How many PSUs do you need.  Hint: sometimes it's two.
-Wire up an example switch (from Amazon).  Test.  How much power is at the terminals now?  Same?  Is the illuminated switch consuming anything that affects your already thin margin on the PSU?
-Add an enclosure as appropriate, e.g. show digital voltmeter example so that you can always tell if you are 'running low'
-Adding fans and other 'always on' elements.  How much is left for the board/motors/heatbed/extruder?  Did that LED array run that all down?
-Unplug the PSU, plug in USB to the board.  Note the board has power, and you can see it, but can't control anything.  Emphasize the point that USB provides power to the board, so you are not really powered off unless the PSU is off/switched off AND the USB is unplugged
-Plug everything back in.  Does everything work?  Can you jog the axes, can you heat the bed, can you extrude?  If anything doesn't respond, power off and disconnect those parts DIRECTLY wired to the PSU one at a time and try again, until you find the power draining culprit: Hint: it might be that big LED array....



## Authors

If you contribute to this video in any way, please add your name to this list : 

* Arthur Wolf
* Samer Najia

