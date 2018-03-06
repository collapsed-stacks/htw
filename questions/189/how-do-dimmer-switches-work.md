## How do Dimmer switches work?

- posted by: [Noctrine](https://stackexchange.com/users/-1/50-noctrine) on 2011-04-19
- tagged: `electronics`, `household`
- score: 3

I noticed that dimmer switches just work when installed. How do they work, or what allows any light to work with a dimmer switch?


## Answer 193

- posted by: [e.James](https://stackexchange.com/users/-1/54-e-james) on 2011-04-19
- score: 4

<p>A dimmer switch changes the brightness of a light by increasing or reducing the amount of electrical power that reaches the light. This is accomplished by <a href="http://en.wikipedia.org/wiki/Modulation" rel="nofollow">modulating</a> the voltage to the light.</p>

<p>The dimmer essentially flips the light on and off many times per second (fast enough that the human eye does not notice any flicker). To make the light brighter, the switch stays in the "on" state more than in the "off" state. To dim the light, the switch stays in the "off" state more than in the "on" state.</p>

<p>Switch in the "full on" state:</p>

<pre><code>     |
 ON -+ --------------------------------------------
     |
     |
     | 
OFF -+
     |
     +---------------------------------------------&gt; (time)
</code></pre>

<p>Switch in the "full off" state:</p>

<pre><code>     |
 ON -+
     |
     |
     | 
OFF -+ --------------------------------------------
     |
     +---------------------------------------------&gt; (time)
</code></pre>

<p>Bright light:</p>

<pre><code>     |
 ON -+   +-----------+   +-----------+   +-------
     |   |           |   |           |   |
     |   |           |   |           |   |
     |   |           |   |           |   |
OFF -+ --+           +---+           +---+
     |
     +---------------------------------------------&gt; (time)
</code></pre>

<p>Dim light:</p>

<pre><code>     |
 ON -+      +---+           +---+          +-----
     |      |   |           |   |          |
     |      |   |           |   |          |
     |      |   |           |   |          |
OFF -+ -----+   +-----------+   +----------+
     |
     +---------------------------------------------&gt; (time)
</code></pre>



## Answer 213

- posted by: [starblue](https://stackexchange.com/users/-1/107-starblue) on 2011-04-19
- score: 4

Voltage and current of AC electricity have the shape of a sine wave with 50 or 60Hz (cycles per second), depending on where you are. So there are 100 or 120 half-waves each second. A typical dimmer for incandescent lamps "cuts off" a leading part of each half-wave to dim the light, so that only the remaining part reaches the light.

Not every light works with a dimmer. It might not work if the light contains some electronic circuit that is not designed for dimming, for example some <a href="http://en.wikipedia.org/wiki/Compact_fluorescent_lamp#Design_and_application_issues">compact flourescent lamps</a>.





---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
