## This video is about : 

How to provide power from a power supply, to the stepper motor power input, so that steppers can rotate

## This video will teach the following things : 

* You need to watch the power supply video first
* Motors need 12 or 24v power. 24v power is best but 12v is good enough
* You need to provide enough power for your stepper's rating
* You need to use a cable thick enough for the current rating 
* Connect wires to PSU, connect wires to Smoothie VMOT [show]
* Polarity is important, double check and test 

This video is not about : connecting, configuring and using a stepper motor

## Links 

The description for this video should contain the following links : 

* http://smoothieware.org/3d-printer-guide#toc3

Also add any other information that should be added

## Video plan

The video is composed of the following sections : 

* Introduction
* Wiring

## Assets

Assets are pictures and videos to be displayed in the video.
Please here list and describe the various assets. They should be commited to github in this folder.

* One asset
* Another asset

## Video synopsis

Putting some thought into powering your stepper motors is time well spent.  The stepper motor system consist of a stepper motor driver for each motor.  Stepper motors are pretty much useless without a stepper driver.  Most stepper drivers can be powered with 12 volt or 24 volt.  A 12 volt power supply will provide enough power to get you started and support standard automation requirements.  Once you are more familiar with powering your build you should take some time to review 24 volt power supply.  Here are some of the benefits gained using 24 volts. {add link to 12/24 volt comparison benefits}

Its also important to use the correct size wire that will connect the stepper motor driver to the stepper motor.  Having wires that are too small will cause the wires to become hot and it could turn into a safety issue.  For a typical NEMA 17 stepper rated at 1.5 AMPS per phase a cable size of 22AWG should work fine to get started.  Just remember adjust your cable size if power requirements change for your motor or power supply.

If your intended application for the stepper motors requires intricate detail control then you should also consider twisting or braiding each set of cables.  The reason is due to something called EMI (Electromagnetic interference).  To explain this, remember back in grade school when the teacher wrapped wire around a nail and then connected it to a battery?  Well I was not paying attention when this happened but someone told me it turned the nail into a magnet!!!  Neat!  This is the same thing that happens when you have current flowing through cables laying next to each other.  In cases where fine detail control is needed EMI can cause problems and show up in the engraving, cutting or extruding.  From a logical perspective it just makes sense to twist or braid your wires since it does not introduce any risk to the operation of monitor and control.

{show backend of a 12v PSU with 14 AWG}
{show VMOT with same wires connected to PSU}

Explain polarity and how to test


## Authors

If you contribute to this video in any way, please add your name to this list : 

* Arthur Wolf
* Mark Ingle

