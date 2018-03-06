## What can possibly break in an electronic device with no moving parts?

- posted by: [Pavel Radzivilovsky](https://stackexchange.com/users/-1/127-pavel-radzivilovsky) on 2011-04-19
- tagged: `electronics`, `failure-mode`
- score: 5

if a device is maintained according to the manufacturer's instruction, i.e. never overheated, kept at right air pressure and humidity, does it still have a way to fail?



## Answer 169

- posted by: [starblue](https://stackexchange.com/users/-1/107-starblue) on 2011-04-19
- score: 4

Electrolytic capacitors dry out over time.

Flash memory wears out after too many erase cycles.

LEDs become less bright over time.

Things can happen that the manufacturer didn't anticipate. For example, <a href="https://secure.wikimedia.org/wikipedia/en/wiki/Tin_whiskers">tin whiskers</a> can form due to reasons not completely understood.


## Answer 165

- posted by: [Locke](https://stackexchange.com/users/-1/108-locke) on 2011-04-19
- score: 2

The most common I can think of is a power line transient: spurious voltage spikes on a power line that can produce component breakdowns. But there are other things that can break an electronic device; For example: a faulty capacitor, a soldering defect, etc...


## Answer 163

- posted by: [shellholic](https://stackexchange.com/users/-1/128-shellholic) on 2011-04-19
- score: 1

I see:

- planned obsolescence
- bad luck (one of the pieces was outside the three-sigma rules)
- time (oxidation, irradiation)
- lie / bad instructions
- unnoticed event (short power failure,...)


## Answer 168

- posted by: [Tangurena](https://stackexchange.com/users/-1/74-tangurena) on 2011-04-19
- score: 1

All materials expand at different rates when temperatures change. Even if you think you keep them at a constant temperature, there are small (sometimes large) and measurable temperature differences across circuit boards, which produce stresses on all the connections. ROHS-compliant solders (lead-free) are more brittle than the old lead-based solders so the connections are more likely to break and make intermittent connections on newer electronics than older stuff. 


## Answer 345

- posted by: [Jason S](https://stackexchange.com/users/-1/77-jason-s) on 2011-04-23
- score: -1

<p>Look up <a href="http://en.wikipedia.org/wiki/Failure_rate" rel="nofollow">failure rate</a> and <a href="http://en.wikipedia.org/wiki/Bathtub_curve" rel="nofollow">bathtub curve</a> and <a href="http://www.itl.nist.gov/div898/handbook/apr/section1/apr151.htm" rel="nofollow">Arrhenius equation</a> in Wikipedia or Google.</p>

<p>Reliability engineers model the failure of various components as probabilistic process where the failure rate is a function of time or temperature or stress (electrical or mechanical).</p>

<p>In electrical components, any form of use tends to cause <em>some</em> electrical stress in the component. Capacitors and semiconductors undergo stress with applied voltage. Power semiconductors expand and contract when they heat up and cool down due to switching on and off. So even if the part isn't moving, it can undergo stress that causes a small but finite chance of component failure.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
