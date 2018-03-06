## How do cell phones and other wireless networks operate without interfering with each other? 

- posted by: [Faisal Abid](https://stackexchange.com/users/-1/85-faisal-abid) on 2011-04-19
- tagged: `electronics`, `radio`, `internet`, `cell-phone`
- score: 3

I've always wondered how radio signals works, for example in cellphones or router to a laptop. How does a phone or laptop or etc know which signal to pick up and read? I know each phone is set to a certain frequency, but isn't that frequency the same for each phone, and if not then how many possible frequencies can you have? 


## Answer 108

- posted by: [EvilPhoenix](https://stackexchange.com/users/-1/78-evilphoenix) on 2011-04-19
- score: 4

<p>A cell phone picks up on a standard radio signal from a cellular tower.  The frequencies at which cellular towers operate varies between wireless providers, whose phones have programming to listen for only their specific frequencies.  These frequencies are shared by the phones, and those phones each have an individual identification code of some type (this varies between cellular providers) which the tower detects, and then, similarly to the way that your computer communicates on the internet, the communication of data is transferred to your device and the cellular towers.  The identification codes (along with your cell phone's number) are used in the communication of the data between phone-and-tower, which is how your signals do not get mixed up with the signals of another phone.</p>

<p>Wireless computer signals operate under similar contexts, however there are several additional concerns.  Wireless signals for routers all operate with a base frequency of 2.4GHz.  The various wireless standards (B / G / N) each operate with different channels, which are just minor offsets of the 2.4GHz frequency, however the frequency of a channel never goes beyond 2.5GHz.  This image courtesy of Wikipedia has a decent visual explanation of the differences of channels across the various wireless internet standards:<br>
<img src="http://i.imgur.com/IiFyo.png" alt="Wireless Channels"></p>

<p>Along similar lines as that of phones, wireless computing devices have individual hardware identification codes, called MAC addresses, which identifies to a router your individual network device.  This information is stored in the router, which has its own hardware identification code, as well as an ID on the internet (an IP address) which establishes the starting point of data transmission, and is utilized by your router to identify incoming data (and outgoing data) as being destined to your computer.  Similarly, routers and internet hubs around the world will act as junction points between your internet and the site or location of your information that you are requesting.  The communication at the destination end is similar to the communication between your router and your computer, except that the destination is typically one box rather than a router-to-computer system.  The data is sent back from the remote system, follows the steps that the data took to get to itself, and the data ends back up at your router, which in turn identifies the information from the remote source, and knows that your computer requested it.  This information is sent from your router back to your computer, where the various data (which is in tiny segments of information called "packets") is reassembled in order by your computer.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
