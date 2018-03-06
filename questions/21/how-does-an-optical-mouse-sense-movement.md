## How does an optical mouse sense movement?

- posted by: [Josh](https://stackexchange.com/users/-1/20-josh) on 2011-04-18
- tagged: `computers`, `computer-hardware`, `optics`
- score: 9

I've been using mice since they had mouseballs. I know how mice with mouseballs worked -- they had small rollers for the X and Y axes and these were connected to rings with slots, which allowed light to pass onto a sensor as they turned, allowing the movement to be converted into electrical signals. But how do **optical** mice work? That is, newer mice which only use light to sense motion. What actually happens as you move an optical mouse? 


## Answer 33

- posted by: [Jacob](https://stackexchange.com/users/-1/28-jacob) on 2011-04-18
- score: 5

It works like a camera. It takes about 1500 images a second with a red LED that bounces off a CMOS ( complimentary metal-oxide semiconductor) that transfers the images to the digital signal processor. The DSP then tracks slight movements and is able to compare those differences to see how the mouse moved. 


## Answer 32

- posted by: [MalsR](https://stackexchange.com/users/-1/31-malsr) on 2011-04-18
- score: 4

The main difference between a traditional 'wheeled' mouse and an optical mouse is the optical mouse has a red light emitting diode (LED), the optical eye! that will bounce light off a surface onto a semiconductor. This sensor sends each image to a DSP (digital signal processor) where it detects the patterns and examines how the patterns have moved since the previous image.  

It can pick up very fine differences in the images and from this it can determine how far the mouse has moved across your desk and at what speed. Here coordinates are then sent to the computer which moves the cursor on the screen!



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
