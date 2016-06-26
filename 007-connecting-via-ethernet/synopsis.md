## This video is about : 

How to connect via Ethernet, configure and use the network stuff.

## This video will teach the following things : 

* Why Ethernet over USB
* What Ethernet gives you
* How to wire
* How to configure on Smoothie's side ( static, DHCD )
* How to setup your network ( router or crossed cable )
* How to connect ( telnet, http )
* Troubleshooting

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
* Usage
* Troubleshooting

## Assets

Assets are pictures and videos to be displayed in the video.
Please here list and describe the various assets. They should be commited to github in this folder.

* One asset
* Another asset

## Video synopsis

There are two main ways of communicating with your Smoothieboard : USB and Ethernet.

Ethernet [http://smoothieware.org/network] is very much recommended, since it is much less likely to have disconnection troubles, compared to USB. Also, it doesn’t require installing a driver on Windows like USB does.

To use Ethernet, you first need to get an Ethernet cable, and connect the Smoothieboard to your local network.

This is the same as connecting a new computer or a new 2D printer to your local network {show cable connection}

Then, you need to tell Smoothieboard that you want it to talk over the network.

This is done by editing the configuration file, and changing the network.enable option from false to true.

Once this is done, reset the board. The board will now automatically connect to your network, and obtain an IP address via DHCP.

All computers and peripherals on your local network have an IP address. In order to talk to your Smoothieboard, you need to find it’s current address.

There are several ways of doing so : 

If you have a panel connected to the Smoothieboard, the panel should display the IP address {demonstrate}
If you have access to your network’s main router’s administration interface, it should tell you the IP address of all peripherals connected to it {demonstrate}
If you are connected to the board via USB, you should be able to use a program like Pronterface to send the “@net” command, which gives you the current IP address. {demonstrate}
If you are running linux, you can use a command like nmap -sn 192.168.0.0/24 {show on screen} to find all acessible peripherals on the network. {demonstrate}

Once you know your Smoothieboard’s IP address, type it in the address bar of your web browser {demonstrate}, and you should be able to access the web interface for the Smoothieboard.

Alternatively, you can also use a program like Pronterface [http://smoothieware.org/pronterface] to talk to the board via the network. {demonstrate}

If you like, you can also use telnet to get a “raw” serial interface to the board {demonstrate}.

### Static IP

The default method is to automatically get an IP via DHCP, but you can also specify a static IP address by yourself.

Make sure the IP is in the correct range for your network ( for example by looking at your computer’s IP addresŝ ), and that it is not used by anything else.
Then you can specify the address [http://smoothieware.org/network]
{show config for this case}

### Troubleshooting

If you know the IP address for your Smoothieboard, but the board is not answering, try resetting it, using another browser, or using pronterface instead of a browser.

 If none of these work, try contacting the community.

## Authors

If you contribute to this video in any way, please add your name to this list : 

* Arthur Wolf

