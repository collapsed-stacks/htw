## How does a flatbed scanner work?

- posted by: [mgkrebbs](https://stackexchange.com/users/-1/139-mgkrebbs) on 2011-04-19
- tagged: `electronics`, `computers`, `computer-hardware`, `optics`
- score: 6

Modern scanners are quite inexpensive yet manage to deliver quality images at high resolutions (e.g. with each pixel covering only 1/1200th of an inch!).

A flatbed scanner clearly has an arm that slowly travels the length of the glass bed and carries a light to illuminate the photo or document.  Is there one sensor or many?  Are the sensors the same as in a digital camera? Does the sensor move or are there mirrors or lenses that focus light from the part of the document being scanned?  How do they manage to get such fine detail when there are mechanical components shuttling about?  Does the scanner partly overlap on successive scan passes and somehow match the overlapping image with the previous part in order to achieve precise registration at high resolution?


## Answer 208

- posted by: [mgb](https://stackexchange.com/users/-1/15-mgb) on 2011-04-19
- score: 4

The sensor is a linear CCD - essentially the same as in your digital camera but only a single row of pixels across the page.   

The accuracy in the along the page is done by simply driving the scanner at a fixed speed, with a stepper motor, and reading at a certain rate - then assuming that you know the exact position at the moment that a pixel was readout.

The scan resolution is (at least on consumer units) a bit of an exageration. 

They claim 1/1200th of an inch but that doesn't mean they can resolve lines 1/1200th of an inch apart - it usually means that they take a reading every 1/1200th inch, or more likely  they take a reading less often and interpolate. 
The optics are unlikely to be good enough to be measuring a single spot 1/1200inch across.


It's like ink jet printers that claim 1000dpi but put down drops which are 1/100inch in diameter.




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
