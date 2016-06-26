## This video is about : 

This is the first video in the series, it's intended to explain what is Smoothie, give general pointers on documentation, and a word of warning on safety.

## This video will teach the following things : 

* What is the Smoothie project ( community-made, not a classical "product" )
* What is Smoothieboard
* What is the Smoothie firmware
* Where to find information ( smoothieware.org )
* Where to get help and get in touch with the community
* You can damage yourself doing this stuff

## Links 

The description for this video should contain the following links : 

* A link
* Another link

Also add any other information that should be added

## Video plan

The video is composed of the following sections : 

* What is Smoothie ?
* Where to find information ?
* What makes Smoothie special ?
* Where to find help ?
* A word on safety.

## Assets

Assets are pictures and videos to be displayed in the video.
Please here list and describe the various assets. They should be commited to github in this folder.

* One asset
* Another asset

## Video synopsis

Welcome. 
In this series, we’ll be explaining how to configure, wire, and use a Smoothieboard to control digital fabrication machines like 3D printers, laser cutters and milling routers.

### What is a Smoothie ?

Smoothieboard is a CNC controller. {show board}
CNC, or Computeried Numerical Control [https://en.wikipedia.org/wiki/Numerical_control] is the automation of machines that make things.
By opposition to “manual” control, it allows you ( or software you are using ) to program a machine to do things, and then let it do those things.

Smoothieboard essentially acts like the “brain” of the machine you install it in. 
You connect your computer to the Smoothieboard, and you connect the Smoothieboard to the different elements of your machine ( like motors ), and then you can use your computer to control the machine, and send it lists of instructions to execute ( G-code ).

Very similar to your computer, Smoothieboard is made of a type of processor called a microcontroller, and a set of peripherals {point microcontroller on board}. It’s a computer specially designed for a specific task.

This microcontroller executes a single program, also called it’s “firmware”. For a Smoothieboard, that firmware is called “Smoothieware”, or “Smoothie” for short.
To use your machine, you will need to configure that firmware to fit your specific case.

Both Smoothieboard and Smoothieware are Open-Source projects ( like for example Linux, Wikipedia or Arduino ), created and maintained by a community of volunteers. 
You are free, and very welcome [https://github.com/Smoothieware/], to contribute to the project, use, read, edit and distribute the source code, as well as the board designs.

## What makes Smoothie special ?

There are other Open-Source CNC controller projects, and even more closed-source controller "products".

The main things that set Smoothie aside are : 

* It is meant to be general purpose : instead of being just for 3D printers or just for lasers, the code is designed to accomodate as many uses as possible. The aim is to bring several different communities together to create a stronger project, and so that work in one domain benefits the other domains.
* It is meant to be easy to contribute to : the modular design aims at making it as easy as possible to "add new things" to Smoothie. This is true both for the hardware, and for the firmware. While as a normal user you might think that does not matter to you, it is the reason why the project is so feature-rich. It will actually probably take you some time to realize how many things Smoothie is capable of.
* It is meant to be beginner-friendly : There is a strong emphasis in the project to try to make configuration and use as easy as possible ( no need for compilation for example ), as well as a huge documentation effort. The Smoothie wiki is the most complete documentation of any CNC controller project, by far.
* Cutting-edge hardware : Smoothie tries to use the best hardware possible at any given time. This is true of some other projects too.

### Where to find information ?

The website for the Smoothie project, is Smoothieware.org [http://smoothieware.org]

{show screencast of website}

There you can find an extensive documentation on every aspect of both the firmware, and the board.

There are step-by-step guides for each type of machine {point to guides}, as well as more in-depth documentation for each aspect of using the board {point to documentation summary}.

You definitely want to read the guide for the machine you will be building, {enter a guide, scroll} it is full of useful information.
The guide will generally be sufficient for the more general use cases, but if your machine is doing something special/unusual, then it’s likely that is covered in the rest of the documentation.

And of course, you can watch the other videos in this tutorial series.

### Where to find help ?

The Smoothie community is full of users ready to share tips, and help with any problem you may encounter.

To make sure the time of community members ready to help is used as efficiently as possible, always make sure you check the answer to your question is not in the documentation already.

If you can’t find an answer in the documentation, you can get help in the following places : 

{website screencast again, go to the “community” tab in the top bar}

IRC, {click IRC, connect via the web applet, ask a question } for Internet Relay Chat, can be used to talk directly to a channel and ask your question directly.  [http://smoothieware.org/irc]
If you do not get an answer immediately, be patient, not everybody is present all the time.
It is recommended to ask questions on IRC before asking them anywhere else.

The Forum {go to forum, scroll} allows you to post questions, that are then visible to everybody. Getting answers will take longer than on IRC, check if your post was answered on a regular basis.
You can also browse the forum to see if your question has already been answered in an older post.

The mailing lists {go to support mailing lists} allows you to subscribe to the mailing list ( google group ) and send message to others that have subscribed as well. It is very similar to the forum, but is based on email.

The google+ community {go to G+ community} is yet another way to get help by posting your questions and waiting for answers.

It’s better if you do not post everywhere at once. Choose one way of asking your question, based on your preference, ask your question there, and wait for an answer. If you do not get an answer, or if nobody in the community knows the answer, then you can try asking in another place.
Posting on the forum and the mailing list at the same time, for example, can be a waste of resources because you might get two persons helping you in parallel, when only one was needed.

If you received help, please consider helping others in turn. That is how we keep the project going, we need your help. 

### A word on safety.

While setting up your machine, depending on the type, you might have to deal with : 

Alternating mains power
Heating elements
Lasers
Spindles
Moving parts

All those can be dangerous [http://smoothieware.org/warning]. 

If you are not careful, you could damage your board, but much more importantly, you could damage yourself.
In particular, high voltage can kill you, lasers can turn you permanently blind, heating elements can burn you or start a fire, spindles and moving parts can cut you.
{ Do something a bit extreme to nail this in. Car crash video clip ? }

Please always be very careful what you do. 
If you are not sure about something, stop, step back, and find more information.
If you are not competent to do something, get help.

You are responsible for your own safety. Please, be safe. 

## Authors

If you contribute to this video in any way, please add your name to this list : 

* Arthur Wolf

