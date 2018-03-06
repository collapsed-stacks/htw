## How do contactless smartcards work?

- posted by: [Louis Rhys](https://stackexchange.com/users/-1/92-louis-rhys) on 2011-04-19
- tagged: `wireless`, `transportation`, `smartcards`
- score: 1

![Contactless smartcard][1] 

[Contactless smartcard](http://en.wikipedia.org/wiki/Contactless_smartcard) (example: Mass transit card)

How do these things work? Do they transmit data via some frequency? What is the power source? How does another machine change its data (for example, transportation card balance). And how to make sure people won't duplicate a card or modify the content of a card?


  [1]: http://i.imgur.com/xD0gv.jpg


## Answer 140

- posted by: [xeroc](https://stackexchange.com/users/-1/106-xeroc) on 2011-04-19
- score: 2

The technologie used here is called RFID (Radio Frequency Identification) and - how name tells us - uses wireless techniques to transmit data. There are different types of RFID-Tags (Transponders). Most of them are 'passive' which means they have no power source. Those tags are powered by the electro-magnetic field that is produced by the card-reader.

Each bits is sent by changing the card's transponder's internal resistance, causing more or less power to be extracted from the the magnetic field. The extracted power is then determined by the reader and the sent bit is retrieved. This is basically, how RFID work at a low frequencies.

High frequency RFID (usually UHF - at least here in germany) uses the so called backscatter to transmit data.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
