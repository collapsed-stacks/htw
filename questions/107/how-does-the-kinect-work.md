## How does the Kinect work?

- posted by: [bguiz](https://stackexchange.com/users/-1/88-bguiz) on 2011-04-19
- tagged: `electronics`, `kinect`, `algorithm`
- score: 4

How does the Kinect work?

1. The Kinect uses cameras to detect not only images, but also the "depth" of each part of the image. What is the mechanism by which this works?

2. Once the image and depth-map are obtained, how is it then able to detect the players' (skeletal recognition) movements? Describe, preferably in layman's terms, the algorithms and other technology involved in this translation.

Thanks!!



## Answer 215

- posted by: [Stefano Borini](https://stackexchange.com/users/-1/23-stefano-borini) on 2011-04-19
- score: 2

<p>Kinect is, deep down, a <a href="http://en.wikipedia.org/wiki/Structured_Light_3D_Scanner" rel="nofollow">structured light scanner</a>, meaning that it projects an infrared pattern (so invisible for us). According to the underlying technology firm PrimeSense, <a href="http://research.microsoft.com/pubs/145347/BodyPartRecognition.pdf" rel="nofollow">the structured light code is drawn with an infrared laser</a>. This pattern is then read by an infrared camera and the 3D information is reconstructed from the distortions of the pattern. This results in a depth channel which is made available through USB.</p>

<p>If you want to see the pattern, you may have some luck by turning off all the lights in the room, turn on the kinect, and try to use your cellphone camera. Generally, these camera sensors are sensitive to IR, which appears as green. You may verify if this is the case by trying the same with a TV remote and pressing the buttons. The LED should turn green.</p>

<p>When it comes to recognition of body parts, it uses a so-called decision forest, which has been trained with previous images of different body sizes and positions. When a new image is fed into the decision forest, it is able to infer the positions from the training. Microsoft research <a href="http://research.microsoft.com/pubs/145347/BodyPartRecognition.pdf" rel="nofollow">published a paper on this</a>. <a href="http://www.i-programmer.info/news/105-artificial-intelligence/2176-kinects-ai-breakthrough-explained.html" rel="nofollow">This article goes in a less-technical explanation</a> and <a href="http://www.youtube.com/watch?v=HNkbG3KsY84" rel="nofollow">this video shows the results</a>.</p>



## Answer 111

- posted by: [Pearsonartphoto](https://stackexchange.com/users/-1/67-pearsonartphoto) on 2011-04-19
- score: 0

<p>There is far more to Kinect than meets the eye. Just up front, I got alot of this, but not all of it, from the <a href="http://electronics.howstuffworks.com/microsoft-kinect.htm" rel="nofollow">How Stuff Works</a> website.</p>

<p>There are 3 basic sensors on the Kinect, of which one is active. Namely, they are:</p>

<ul>
<li>Video Camera</li>
<li>Microphones</li>
<li>Active IR sensor</li>
</ul>

<p>The video camera uses standard facial recognition to see who is in the scene.</p>

<p>The magic is in the active IR sensor. Basically, it projects an IR grid onto everything. It can determine from what this grid looks like on you how far away you are. It can also see your general shape. It looks specifically for limbs, hands, feet, head, etc. Basically, you look for something that looks like it fits the right shape, and there's your limb. That's also why if you touch someone else, it can cause some serious issues. </p>

<p>Given that it can detect where you are, it can sense movement of all of the limbs, leading to the detection of motion.</p>



## Answer 196

- posted by: [mgb](https://stackexchange.com/users/-1/15-mgb) on 2011-04-19
- score: 0

<p>Mostly it uses <a href="http://en.wikipedia.org/wiki/Structured-light_3D_scanner" rel="nofollow">structured light</a>.</p>

<p>It projects a grid of (invisible) infrared lines onto you which a camera sees. By looking at where the 2d pattern of straight lines bend it is possible to calculate the 3d shape of the surface that they are projected onto.</p>

<p>You can build something very similar yourself with a <a href="http://www.david-laserscanner.com/" rel="nofollow">laser pointer and a webcam</a></p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
