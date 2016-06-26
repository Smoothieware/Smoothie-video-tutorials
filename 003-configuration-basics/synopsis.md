## This video is about : 

Configuration, what it is and how to use it

## This video will teach the following things : 

* What is the configuration file and what it's role is
* What format configuration is written in
* The concept of modules and creating them in config
* How to access the config file, edit it and send it to the board
* Troubleshooting config problems

## Links 

The description for this video should contain the following links : 

* http://smoothieware.org/configuring-smoothie
* https://wiki.gnome.org/Apps/Gedit
* http://smoothieware.org/configuration-options

Also add any other information that should be added

## Video plan

The video is composed of the following sections : 

* Introduction
* Configuration format
* Modules
* Accessing config
* Troubleshooting

## Assets

Assets are pictures and videos to be displayed in the video.
Please here list and describe the various assets. They should be commited to github in this folder.

* One asset
* Another asset

## Video synopsis

Your Smoothieboard controls your machine. You need to tell Smoothieboard about your machine, so it is able to do that job adequately. 

This is done through configuration [http://smoothieware.org/configuring-smoothie]

Where other systems require you edit source code, compile, upload etc, Smoothie offers a very simplified configuration system.

On your Smoothieboard, there is a microSD card socket {show} in which you insert a microSD card {do so}.
The card comes with your board when you purchase it, and is already filled with useful files.

On that microSD card, is a configuration file ( name “config” or “config.txt” ) {screencast of sd card content in file browser}
When the board turns on ( boots ), the firmware will execute, access that file, read the information it contains, and use that information to configure itself.

This means that to configure everything, the only thing you need to do is access that “config” file, and edit it.

The recommended application to edit the configuration file is Gedit [https://wiki.gnome.org/Apps/Gedit], and though any basic text editor should theorically do the job, please be warned that the very popular Notepad++ sometimes does weird things to the file.

### Configuration format

If you open the configuration file with a text editor {do so}, you can see it looks like this.

Each line is made out of a configuration option’s name, followed by it’s value {show}

The file can also contains comments. In the configuration file, anything after the character #, on a given line, will be ignored. Those are comments.
You can see, for example, comments at the end of nearly each line.
You can also see lines that start with #, and are a comment line.

Please note that some lines contain a configuration option and it’s value, but start with a #. Those lines are “commented out”. 
They will be ignored by Smoothie. 
They are generally here as an example. 
You can make the line “visible” again to Smoothie by removing the # at the beginning.

You can use this to disable things without completely remove the line, or to add information to your config file for yourself to remember.

The values for each configuration option, can be numbers {show}, true/false values {show}, GPIO pins {show} or strings of characters {show}, depending on the option.

Smoothie is extremely configurable, a lot of things can be changed. However, the example configuration comes with a lot of reasonable defaults, so it is likely you will not need to edit a lot of the configuration to get things working. Sometimes only editing a handful of values is sufficient.

Do not edit an option if you do not understand what it does. 
Do not “tune” values before your machine works.
When first getting your machine to work, edit as few values as you can. Experimentation is something you should do once everything is working. 
After editing a value, test that it did what you thought it would, before editing another value. This ensures you can identify problems easily if there are any. 

### Modules

Smoothie is a modular firmware. Every functionality is separated into separate pieces called “modules”.

What this means to you, is that if you want to get your machine to control a laser for example, you will be enabling the laser “module” in the configuration {show}. This will cause laser-controlling code to execute.

Some modules can be enabled multiple times. 
For example, if your machine has three extruders, you will be enabling three extruder “modules” {show} in your configuration file ( giving each a separate name {show} ).
Same goes for temperature control modules, or so-called “Switch” modules.

This will be explained in more detail for each module later-on.

### Accessing config

Your configuration file is stored on your microSD card. There are different ways to access this file and change the values in it : 

You can take the SD card out of your Smoothieboard, and plug it into your computer {show}
You can connect via a USB cable, in which case the Smoothieboard acts like a mass storage device, allowing you to access the files {show}
You can connect via the Ethernet cable, and use the web interface to access the configuration file {show}
You can connect via USB/Serial, or via Telnet and use commands to change values in the file

In all cases, once you edited your file, you need to reset the Smoothieboard before the changes will be taken into account.

### Troubleshooting

If you are modifying values in your configuration file, and it has no effect, make sure that value is not overriden by the config-override file [http://smoothieware.org/configuring-smoothie]

If that is not the case, then you should try formatting your card, and copying the files to it again [http://smoothieware.org/sd-card]


## Authors

If you contribute to this video in any way, please add your name to this list : 

* Arthur Wolf

