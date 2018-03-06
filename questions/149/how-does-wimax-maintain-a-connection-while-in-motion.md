## How does WiMAX maintain a connection while in motion?

- posted by: [somehume](https://stackexchange.com/users/-1/10-somehume) on 2011-04-19
- tagged: `networking`, `internet`, `wimax`, `4g`
- score: 3

How is it that I can be a passenger in a vehicle while traveling long distances, such as county to county on I-95 and not lose my connection?


## Answer 198

- posted by: [mgb](https://stackexchange.com/users/-1/15-mgb) on 2011-04-19
- score: 2

Essentially the same as (digital) mobile cellular phone.

You are connected to a local cell, as you move the signal received by your current cell will get weaker and that at the next cell will get stronger.  

At some point the system 'hands over' to next cell and your phone will drop the connection to the previous one and be given a new frequency band to talk to the new cell. The upstream system will be updated that you are now talking to a new cell and all the traffic to you will be routed to the next cell's base station



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
