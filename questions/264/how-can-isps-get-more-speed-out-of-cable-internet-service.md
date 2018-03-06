## How can ISPs get more speed out of cable internet service?

- posted by: [Josh](https://stackexchange.com/users/-1/20-josh) on 2011-04-20
- tagged: `networking`, `internet`, `cable`
- score: 4

I have internet service through my cable company using a cable modem. I'm currently paying for the "turbo" service which gives me ~30Mbps download speeds. When the connection was installed, the technician said that soon they would have an even faster service, up to 60Mbps. He said they're still rolling this service out, and after a certain date if I was interested I should call and get it added to my account.

How does this work? Where does the additional bandwidth come from? What is the cable company actually doing to roll out this service? How can ISPs get more speed out of cable internet service like this?


## Answer 269

- posted by: [Jacob](https://stackexchange.com/users/-1/28-jacob) on 2011-04-20
- score: 4

<p>Cable internet is extremely similar to DSL in that TV channels don't use all the frequencies spectrum in a coax cable. Nearly all systems use the DOCSIS standard for cable internet(Data Over Cable Service Interface Specification) Each regular channel(not compressed through digital MPEG encoders) only take up around 6MhZ each. This can further be reduced with a digital box that decodes M-PEG streams to fit more into a 6MhZ slice. In cable the 5-65MhZ is set for upstream data, and 850-1000MhZ is for down stream. Notice that like DSL this is asymmetric in that your Download and upload aren't the same. The biggest reason for this is that it is assumed that consumers will download more than they upload.(and usually right too.) A cable modem is similar to a DSL transceiver in that it will choose a block to communicate on that is clear of other traffic in the ranges I listed above. Now each of these "channels" allows ~30Mbits of data. I'll explain how you get more in the next section </p>

<p>How does the speed increase with upgrades? Well the DOCSIS standard allows Channel bonding, where your modem can use multiple channels to send and receive more data. DOCSIS 3.0, the newest standard allows a unlimited amount of channels to be used, meaning that is up to the ISP to have the equipment to support all these channels, and the backhaul that is required. This is where cable "slowdowns" occur if the ISP doesn't keep the backhaul , the node equipment up to date or oversubscribes, or even a combination of the three, then the node can't support all the users and your internet slows as a result.  </p>

<p><a href="http://en.wikipedia.org/wiki/DOCSIS" rel="nofollow">Here</a> is a link for the DOCSIS standard, and <a href="http://en.wikipedia.org/wiki/Cable_Internet_access" rel="nofollow">this</a> one is for cable internet in general.</p>



## Answer 266

- posted by: [mgb](https://stackexchange.com/users/-1/15-mgb) on 2011-04-20
- score: 3

The maximum speed on a cable with the current DOCSIS protocol is around 30Mb/, the new version allows up to 4 (IIRC?) of these channels on a single cable - although they may not implement all of them.

So to upgrade you from 30Mb to 60Mb they simply have to fit new equipement in their cabinet and give you a new modem - or possibly just update the firmware if the equipement is new enough that it was built with this capability.

BUT (and it's a big BUT) this only gives you more bandwidth between your home and the nearest cable distribution cabinet - that could still be linked to the rest of the internet by a bit of wet string (if you are on Shaw) - you will still be limited by their total bandwidth to the site you are interested in.






---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
