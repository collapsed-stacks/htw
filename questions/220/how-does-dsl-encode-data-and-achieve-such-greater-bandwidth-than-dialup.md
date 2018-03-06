## How does DSL encode data and achieve such greater bandwidth than dialup?

- posted by: [Josh](https://stackexchange.com/users/-1/20-josh) on 2011-04-20
- tagged: `electronics`, `electricity`, `networking`
- score: 5

How does DSL internet service work? My understanding is that it uses a traditional phone line.. yet, provides much higher speed than dialup. Is it just a standard telephone line and, if so, how is it able to provide such greater speed?

Also, I have head that DSL speed varies based on how far you are from the source... is this true and if so, what causes it?


## Answer 222

- posted by: [Jacob](https://stackexchange.com/users/-1/28-jacob) on 2011-04-20
- score: 4

<p>DSL stands for Digital Subscriber line. The basics are similar to Powerline in that voice doesn't use all of the frequencies possible on the line. Telephones use the first 4KhZ in the system. Have you ever gotten a filter to put on your phones? There call Low pass because they block everything above 4KhZ which is the data range so it doesn't affect voice. This leaves ~247 4KhZ frequencies for DSL data to use. The upstream channel is carried in a band between 25 and 160 KHz. The downstream channel begins at 240 KHz and ends on several factors which I'll touch on later. Your modem(DSL transceiver) will scan these ranges and find the clearest one to use, and it will keep scanning to see if one becomes clearer. For there at the office you connect to the DSLAM (Digital Subscriber Line Access Multiplexer {pronounced D-SLAM} ) which connects you to the internet, normally through a fiber connection from that point on. </p>

<p>Back to the frequencies, notice how the farther you are from the utilities CO or office with the receiving equipment your internet speeds are slower? This is because at the >240KhZ range signal quality begins to degrade heavily due to distance, interference and other factors. Due to this fact, you can usually on get the max speed of DSL ~6000 wire feet out and the maximum transmission is about 18000 wire feet. Notice that that is "wire distance" not the actual distance to the CO. Again this depends on certain factors such as interference, wire condition and  if there are any bridge taps( extend the line, but cause interference >4KhZ.</p>

<p>Check out <a href="http://en.wikipedia.org/wiki/Digital_Subscriber_Line" rel="nofollow">this</a> for more info on DSL, and <a href="http://en.wikipedia.org/wiki/Digital_Subscriber_Line_Access_Multiplexer" rel="nofollow">this</a> for more on the DSLAM equipment</p>



## Answer 304

- posted by: [Christopher](https://stackexchange.com/users/-1/129-christopher) on 2011-04-21
- score: 1

<p>Digital Subscriber Line technology exploits the fact that on a standard POTS telephone line voice doesn't use all of the possible frequencies; speech calls use the first ~3kHz (300Hz-3400Hz). The microfilters you need to install on every telephone socket before you plug in your modem (or Customer Premises Equipment) are lowpass filters - they separate voice frequencies and DSL frequencies (everything above 4kHz) and prevent 'crossover' between the two transmissions.</p>

<p>After filtering speech frequencies, this theoretically leaves ~255 'tones', channels of 4312.5Hz each, for DSL data. ADSL1 and ADSL2 employ a smaller frequency range than ADSL2+ and ADSL2+ with Annex M (which I will explain further); a more detailed breakdown of the frequencies used can be found on <a href="http://www.kitz.co.uk/adsl/adsl_technology.htm#frequencies" rel="nofollow">Kitz's ADSL FAQ site</a>.</p>

<p>Like ADSL1, with ADSL2+ the upstream channel starts at 25kHz and is carried in tones 5-31. However, tone 0 is not used, 1-5 are designated as POTS Guard Bands to avoid crosstalk and 16 is the Pilot Tone. As with ADSL1, ADSL2's downstream channel begins at 142.3kHz (tone 33) and continues up until the attenuation on the line worsens the SNR - the modem decides at which point it should stop attempting to use tones, and this is the basis of your "sync speed" with the exchange. ADSL2+ with Annex M (sometimes called "upload plus"), the upper limit of tones used for the upstream channel is increased from 31 to 56 (with the start tone for the downstream channel moved up accordingly) which provides for a theoretical increase in upstream speed from 1.3Mbps to 2.5Mbps under good conditions. As lower tones are less susceptible to interference or attenuation, a long line with Annex M will typically retain a disproportionately high upstream speed even if the downstream suffers through attenuation or loss.</p>

<p>At the exchange (or CO) your modem communicates with a DSLAM (Digital Subscriber Line Access Multiplexer, pronounced "D-SLAM") - once your traffic is inside the exchange, it is typically passed onto your ISP's backhaul from the exchange to their core network, usually over fibre. With VDSL (sometimes known as FTTC) the DSLAM is just moved closer to your house, usually installed in green or grey street cabinets thereby shortening the length of copper between you and the equipment and providing the additional benefit of lower attenuation and higher sync speeds, which allows for a much greater throughput on the line.</p>

<p>DSL suffers on long or poor quality lines - internal wiring is as important to maintain as external wiring (which in the UK is the property and responsibility of British Telecom). Any unshielded internal wiring will act as an antenna, picking up RF interference and likely also reducing the maximum achievable sync speed. For that reason, having the modem connected to the master socket by as short a run of cable as possible - then running longer ethernet cables to your destination - is a vastly preferable practice. </p>

<p>With regards to how DSL achieves such greater bandwidth, it's a combination of highly efficient error correction and encoding combined with the greater raw bandwidth utilised by the technology over standard analogue V.92 modems. ADSL employs both Reed-Solomon and Trellis Coded Modulation for different ranges of data to accommodate for line noise, interference and LOS. In the UK and some overseas countries, ADSL data is commonly transmitted inside <a href="http://www.kitz.co.uk/adsl/data_transmission.htm" rel="nofollow">ATM cells</a> as PPP frames - the protocol known as PPPoA (RFC 2364). PPPoA is also advantageous as the customer's router can be required to authenticate to the ISP's <a href="http://en.wikipedia.org/wiki/Broadband_Remote_Access_Server" rel="nofollow">BRAS</a> with a valid username and password prior to obtaining Internet access. The other advantage of using PPPoA encapsulation is that it provisions for Header Error Checking and Forward Error Checking (part of the interleaving technology) which further stabilises throughput on problematic lines. The other main protocol of data transmission is PPPoE, but explanation of this technology is beyond the scope of this answer. PPPoE is not commonly used in the UK due in part to historical reasons and also due to complexities arising from mixing the two standards on a national network. </p>

<p><a href="http://www.kitz.co.uk/adsl/interleaving.htm" rel="nofollow">Interleaving</a> is usually applied by default to the data (which increases its resilience to interference, but raises the latency slightly). Clueful ISPs, at least in the UK, will disable interleaving upon request - putting the line into "fastpath" modem - which increases its susceptibility to LOS from interference but can almost halve the RTT, making a connection far better suited for VoIP or online gaming where low latency is very important.</p>

<p>Further reading: <a href="http://www.kitz.co.uk/adsl/equip.htm" rel="nofollow">Kitz.co.uk's ADSL FAQ pages</a> for a lot of detailed information about many aspects of DSL, <a href="http://en.wikipedia.org/wiki/Digital_Subscriber_Line" rel="nofollow">this</a> Wikipedia article for more on the DSL specification and <a href="http://en.wikipedia.org/wiki/Digital_Subscriber_Line_Access_Multiplexer" rel="nofollow">this</a> for more on DSLAM equipment.</p>



## Answer 270

- posted by: [mgb](https://stackexchange.com/users/-1/15-mgb) on 2011-04-20
- score: 0

Remember the phone line is a real wire (at least between you and the exchange) you can push as much bandwidth down it as you like - upto the limit of noise.

At the exchange the speech is digitized, on voice a phone typically 8bits at 8Khz = giving 64kb/s  
  
56K modems basically transferred the computer data in the same format as the digitized speech, along with a special code which said "this data is already digitized just pass it on". The 56K limit is because 1 of the 8 bits was needed to flag this data so 7x8Khz = 56kbit/s




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
