## How do RFID door lock systems work?

- posted by: [Slipstream](https://stackexchange.com/users/-1/39-slipstream) on 2011-04-18
- tagged: `radio`, `wireless`, `locks`
- score: 4

How do RFID (contactless) cards work? Where does the power come from when opening a door lock with an RFID card. I can't imagine there being a battery in the card, and there are no wires leaving the door lock for power supply. I know the system we have, you can update who's card will open which door online, but how do the door locks communicate with the central list, and work out who is allowed through the door?


## Answer 60

- posted by: [geoffc](https://stackexchange.com/users/-1/34-geoffc) on 2011-04-18
- score: 3

Usually the door locks DO have power, and a battery to back them up, and they cache the authentication information they have seen in case their network connection drops. 

There is a loop in the card that is non-powered, but when passed by an electric field reacts in a predictable pattern.  Thus each card can be made to encode a different value.




## Answer 141

- posted by: [Brad](https://stackexchange.com/users/-1/59-brad) on 2011-04-19
- score: 3

The door locks are powered.  In one building where I worked, they refused to open during a power failure.  We all had to walk around to the front desk.  (It was the day after layoffs too, so everyone was worried that HR had expired their badge!)

RFID tags can be completely passive, merely sending out a simple number (well, a precise frequency) in response to a broad spectrum request.  Imagine a tuning fork - the cardreader sends out an all-frequency "chirp" and listens to see who is resonating back.  This is not high security, as anyone with a scanner could duplicate your card by hiding in the bushes.

Larger RFID tags (like car toll tags) may contain a battery that allows them to communicate more interesting data to the toll booth.

Most interesting are tags which are powered by their own antenna.  If the tagreader broadcasts radio emissions on the right frequency, the antenna can draw power from this signal (similar in concept to how an AM radio does not use batteries).  This power can be enough to compute, for example, a key signature based on a private key.  This is the "smart" in your smart credit cards.  They are truly un-duplicatable, even by an adversary who controls the card swipe reader and is listening to all radio traffic.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
