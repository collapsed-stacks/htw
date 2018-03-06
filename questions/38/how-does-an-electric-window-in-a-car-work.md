## How does an electric window in a car work?

- posted by: [MalsR](https://stackexchange.com/users/-1/31-malsr) on 2011-04-18
- tagged: `automobile`, `electric-window`, `window`, `motor`
- score: 3

Recently my car's window just hit the bottom when I used the controls. I found that a metal wire that was connected to the door motor had snapped. How is the motor connected to the metal wire and does the metal wire length depend on the size of the window?


## Answer 66

- posted by: [Pearsonartphoto](https://stackexchange.com/users/-1/67-pearsonartphoto) on 2011-04-18
- score: 0

How this type of thing typically works is as follows:

There's a circuit somewhere which reads in all of the input signals, one from each window. Each motor typically has either 2 or 3 wires that go to it, that connect from the control board to the motor.

In the two wire configuration, there are 3 possible states. Note that the exact combination of raising/lowering depends on the motor.

* **Wire 1= Wire 2**     No change
* **Wire 1> Wire 2**     Will raise window
* **Wire 1< Wire 2**     Will lower window

A more common is a 3 wire configuration. The first two wires contain a constant voltage, one being ground, the other maybe 12 volts. The third line is a control, which depending on how it's set, can tell the window to raise, lower, or stay the same.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
