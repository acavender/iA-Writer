# An unexpected use for a Raspberry Pi

Several months ago, I purchased a [Raspberry Pi][1]. I had three principal uses for it.

I wanted to use it as a [Plex][2] server.

I was also interested in a [Homebridge][3] server, to enable some of my smart devices to work together more effectively.

Finally, I wanted to see if it might be useful when traveling. For longer trips, it makes sense to just take the MacBook Air along. But for short trips of just a few days, could I remote into it if I was traveling with just my iPad Pro and keyboard and needed a full desktop environment for some reason?

I installed [Ubuntu Server 20.04][4], and added the [MATE desktop environment][5], then added the necessary software. Both Plex and Homebridge work great.

The Pi also works well for remote access from the iPad using something like [Jump Desktop][6] or [Screens][7]. It’s understandably a bit slow, given the its specs, but it’s definitely usable.

For the purposes I bought it for, it’s working exactly as expected. 

A few months ago, though, I also found an *un*expected use for it.

I was out of town for an extended period of time, visiting my parents. Before I left, I did some meal prep and stocked my freezer, so I wouldn’t have to think about what to eat when I returned home.

While I was away, there was a nasty storm that took the power out in my area; some who live in neighborhoods very near my own were out for days rather than hours. I needed to know whether the power had gone out at my apartment, if for no other reason than to know whether the food I’d left in the freezer would be safe to eat on my return.

 As it turns out, checking was quick and easy. I connected to the Pi via ssh, and ran:

`uptime -p`

The output showed that the Pi had been running continuously since well before the storm, so I had nothing to worry about.

*Photo credit: [Vishnu Mohanan][8] on [Unsplash][9].*

[1]:	https://smile.amazon.com/stores/CanaKit/page/19109D80-639C-40C8-9222-DC6775C304EE?store_ref=SLP_FW_E1B7FA96-F1B3-477B-819F-11DE24F0A82B
[2]:	https://www.plex.tv/
[3]:	https://homebridge.io/
[4]:	https://ubuntu.com/download/server/arm
[5]:	https://mate-desktop.org/
[6]:	https://jumpdesktop.com/
[7]:	https://edovia.com/en/screens-ios/
[8]:	https://unsplash.com/photos/rZKdS0wI8Ks
[9]:	https://unsplash.com