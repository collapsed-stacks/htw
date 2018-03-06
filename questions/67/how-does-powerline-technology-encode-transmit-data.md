## How does Powerline technology encode/transmit data?

- posted by: [Josh](https://stackexchange.com/users/-1/20-josh) on 2011-04-18
- tagged: `electricity`, `technology`, `networking`
- score: 3

What is the technology at play in the "Powerline" networking technology which allows an Ethernet network to be shared over standard AC wiring? How does this technology work? How far can the signal go? What actually happens to the electric current? I know ethernet uses 8 wires (4 twisted pairs) and the way the cable is set up is essential to the speed and reliability of the connection, so how can this be achieved over a standard wall socket?

What I'm wondering is, what are the actual physics at work? How is data actually transmitted? I understand that standard A/C power lines are 110 volts of alternating current (In the US anyway, 220 in Europe). What happens to the current when using powerline? How is the data actually transmitted?


## Answer 70

- posted by: [Jacob](https://stackexchange.com/users/-1/28-jacob) on 2011-04-18
- score: 3

Powerline works almost like DSL just on powerlines. It uses something called  orthogonal frequency-division multiplexing (OFDM) to split the power line into 84 channels (in the 4.3 MHz to 20.9 MHz), which the adapter can transmit data over concurrently by sending data over the frequencies that are normally unused by power itself. If a power disruption like a surge or noise occurs on a channel it can automatically switch to another channel to reliably transmit data at ~11Mbits. 


## Answer 217

- posted by: [mgb](https://stackexchange.com/users/-1/15-mgb) on 2011-04-19
- score: 1

In simple terms it just puts a small signal voltage on top of the main AC power voltage.

Imagine a circuit that looked at the voltage every microsecond. If the line voltage had gone up from 110V to 112V that's a one, if it had gone down from 112V to 110V that's a 0 - it then just treats those as any other digital data stream.  (For a more correct explanation see the link in Jacob's answer)

Your regular appliances don't notice the extra few volts since the voltage varies by a few volts depending on the time of day and the load anyway.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
