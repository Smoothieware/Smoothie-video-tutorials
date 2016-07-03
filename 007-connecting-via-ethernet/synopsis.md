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

* http://smoothieware.org/network

Also add any other information that should be added

## Video plan

The video is composed of the following sections : 

* Ethernet or USB
* Ethernet benefits
* Wiring
* Configuration
* Static IP
* Usage
* Troubleshooting

## Assets

Assets are pictures and videos to be displayed in the video.
Please here list and describe the various assets. They should be commited to github in this folder.

* One asset
* Another asset

## Video synopsis

### Ethernet or USB

There are two main ways of communicating with your Smoothieboard : USB and Ethernet.

Ethernet [http://smoothieware.org/network] is very much recommended, since it is much less likely to have disconnection troubles, compared to USB, and though USB disconnections are rare, they happen to a few users. Also, it doesn’t require installing a driver on Windows like USB does.

It does however require that you have the necessary equipment to have a wired network ( typically a router ).

### Ethernet benefits

Using the Ethernet connection on your Smoothieboard provides you with several features.

The most important one is the Web server : it allows the Smoothieboard to "serve" web interfaces and applications to you, which you can then use in your favorite browser, on your computer or on your phone, to control your machine {show}.

A secondary feature is the telnet server, which allows you to connect to the board using a telnet terminal, much like you would with a serial terminal. {show}, also allows some host programs like Pronterface or Visicut to connect

### Wiring

To use Ethernet, you first need to get an Ethernet cable, and connect the Smoothieboard to your local network.

This is the same as connecting a new computer or a new 2D printer to your local network {show cable connection} : Plug the cable into the Smoothieboard on one end, and into the router on the other end.

Note that you can't connect the Smoothieboard directly to your computer, at least not using a normal Ethernet cable. You do need a router.

### Configuration

Then, you need to tell Smoothieboard that you want it to talk over the network.

This is done by editing the configuration file, and changing the network.enable option from false to true. {show}

Once this is done, reset the board. The board will now automatically connect to your network, and obtain an IP address via DHCP.

All computers and peripherals on your local network have an IP address. In order to talk to your Smoothieboard, you need to find it’s current address ( that the router automatically assigned it )

There are several ways of doing so : 

* If you have a panel connected to the Smoothieboard, the panel should display the IP address {demonstrate}
* If you have access to your network’s main router’s administration interface, it should tell you the IP address of all peripherals connected to it {demonstrate}
* If you are connected to the board via USB, you should be able to use a program like Pronterface to send the “@net” command, which gives you the current IP address. {demonstrate}
* If you are running linux, you can use a command like nmap -sn 192.168.0.0/24 {show on screen} to find all acessible peripherals on the network. {demonstrate}

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

If you configured the board for DHCP and it is not getting an IP assigned at all, try using a different router if possible. A few router models have been know not to work with Smoothie.

## Authors

If you contribute to this video in any way, please add your name to this list : 

* Arthur Wolf

