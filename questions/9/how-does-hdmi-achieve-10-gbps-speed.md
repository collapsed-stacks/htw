## How does HDMI achieve 10 GBps speed?

- posted by: [Marco Ceppi](https://stackexchange.com/users/-1/14-marco-ceppi) on 2011-04-18
- tagged: `electronics`, `hdmi`
- score: 5

How does HDMI cables achieve 10 GBps speeds?


## Answer 144

- posted by: [bubu](https://stackexchange.com/users/-1/109-bubu) on 2011-04-19
- score: 3

<p>You should first understand what makes an interface.</p>

<p>things like HDMI specifies many things, which includes:</p>

<ul>
<li>connectors (shape, no. of pins, etc.)</li>
<li>qualification of cable (what bandwidth is required - and hence cable characteristics such as gauge, composition, necessity of twisted pair configuration, shielding, etc etc.)</li>
<li>communication protocol (what pins are used by what protocol in what direction, how data is encoded etc.)</li>
</ul>

<p>Basically the thing that allows for HDMI 10GBps speed are:</p>

<ul>
<li>the processing speed of the video DSPs that drives the HDMI interface, and</li>
<li>the quality of the cable, which i will elaborate more on later.</li>
</ul>

<p>The bandwidth of a cable (e.g. 340MHz @DTing mentioned) relies basically on things such as capacitance, resistance and inductance of a cable. you can think of the cable as a L-C-R network (the equivalent of a combination of an <a href="http://en.wikipedia.org/wiki/Inductor" rel="nofollow">Inductor</a>, a <a href="http://en.wikipedia.org/wiki/Capacitor" rel="nofollow">Capacitor</a> and a <a href="http://en.wikipedia.org/wiki/Resistor" rel="nofollow">Resistor</a>).</p>

<p>basically 2 problems occur in high frequency signaling:</p>

<ul>
<li>capacitance --> note that capacitance is related to the </li>
</ul>

<p>Capacitance is related to (1) distance between two wires, (2) dielectric constant of the material between the wires, and (3) the amount of surface area where the electric field develop.</p>

<ul>
<li>inductance</li>
</ul>

<p>Inductance is related to (1) the area between the wires, (2) dielectric, and (3) the current density flowing down the wires.</p>

<p>so for the HDMI cable to be able to carry the high frequency signal, the construction has to be good enough and we need to make sure that the capacitance and inducance are within limits; for example if the wire is too thin, then the skin effect would be very important (because high frequency signals travels only on the surface of the wire, thus surface area is important.. etc..) </p>



## Answer 138

- posted by: [DTing](https://stackexchange.com/users/-1/62-dting) on 2011-04-19
- score: 0

<p>HDMI which stands for High-Definition Multimedia Interface is unable to reach 10GBps (gigabytes per second), however with specification <a href="http://www.hdmi.org/press/pr/pr_20060622.aspx" rel="nofollow"><strong><code>1.3</code></strong></a> HDMI reached 10.2 Gbps (gigabits per second).</p>

<blockquote>
  <p>Higher speed: HDMI 1.3 increases its
  single-link bandwidth from 165MHz
  (4.95 gigabits per second) to 340 MHz
  (10.2 Gbps)</p>
</blockquote>

<p>I'll let someone who is an expert with cables tackle the main question.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
