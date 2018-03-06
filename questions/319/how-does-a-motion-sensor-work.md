## How does a motion sensor work?

- posted by: [cbrulak](https://stackexchange.com/users/-1/160-cbrulak) on 2011-04-21
- tagged: `security`, `motion-sensor`, `reliability`
- score: 1

How does a motion sensor work and how are they tested to ensure they never fail or crash,etc? 


## Answer 322

- posted by: [bubu](https://stackexchange.com/users/-1/109-bubu) on 2011-04-21
- score: 1

I think from the tags you used that you are asking for information about the motion sensors used in security devices.

There are three major types of motion sensors currently in use:

 * passive infrared sensor (detects infrared emitted because of body heat) 
 * ultrasound scanner
 * microwave scanner

The latter two would emit waves and detect change in the response which indicates movement.

Passive infrared sensors are essentially solid-state devices and do not commonly fail prematurely. The testing of these sensors are the usual battery as other equipment. 

More importantly, one should know that all equipment fails. If one is concerned about failure of equipment causing a security breach, one should consider redundancy rather than reinforcing testing procedures. Additionally, any computer used to monitor the motion is much more likely to fail than the sensors.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
