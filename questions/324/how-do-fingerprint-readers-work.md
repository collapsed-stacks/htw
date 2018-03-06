## How do fingerprint readers work?

- posted by: [somehume](https://stackexchange.com/users/-1/10-somehume) on 2011-04-21
- tagged: `security`, `fingerprint`, `biometrics`
- score: 5

I have a fundamental understanding that they scan your finger. How do they accurately scan? How are fingerprints evaluated?


## Answer 326

- posted by: [Josh](https://stackexchange.com/users/-1/20-josh) on 2011-04-21
- score: 5

Some fingerprint readers use [CCD sensors](http://en.wikipedia.org/wiki/Charge-coupled_device) to generate an image of your fingerprint much the same way a digital camera would take an image. These scanners achieve accurate scans by first running a number of tests on the images produced of the fingerprint:

 1. The scanner will evaluate the image and determine if the levels are balanced, that is, if the image isn't too dark or too light.
 1. The scanner will search for straight vertical and horizontal lines of very dark and very light color, and examine these lines to see if they are crisp, to determine if the image is sharp enough

The scanner will re-capture an image repeatedly until it meets all of the above criteria. Once it has a good image, the scanner will parse the image and calculate what are known as [minutiae](http://en.wikipedia.org/wiki/Minutiae), mathematical descriptions for shapes and patterns in an image, specifically of a fingerprint.

The minutiae which are captured from the scan of your fingerprint are compared with a  database of known authenticated minutiae from when the scanner was set up. If a strong enough match is found, you are considered authenticated.


## Answer 325

- posted by: [geoffc](https://stackexchange.com/users/-1/34-geoffc) on 2011-04-21
- score: 3

There are many approaches.  One is to look at the scanned image of the finger print, and decide via some algorithm how to describe the finger print uniquely.  That is, not scan the whole thing and store but calculate some value for it, and then store that value.

Some actually scan and store the entire image.

There was a great article on Heise.de about defeating them with gummy bears, since the residual grease left behind with a warm mushy gummy bear, can look a lot like a finger print. 

Mythbusters did a great episode on trying to defeat some of them using photocopies of a fingerprint taken from a glass, and also using other approaches. 



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
