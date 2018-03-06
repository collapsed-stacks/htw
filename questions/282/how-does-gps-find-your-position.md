## How does GPS find your position?

- posted by: [Jacob](https://stackexchange.com/users/-1/28-jacob) on 2011-04-21
- tagged: `electronics`, `computers`, `technology`, `engineering`, `gps`
- score: 2

We've all been lost before, we then grabbed the nearest GPS Device and BAM, we know where we are. How does GPS work, how is it able to maintain a high level of accuracy?   


## Answer 283

- posted by: [Pearsonartphoto](https://stackexchange.com/users/-1/67-pearsonartphoto) on 2011-04-21
- score: 3

Imagine that you lived on a line, and there were two points that broadcast themselves ever second, traveling at a speed of, say, a mile per hour. If you knew exactly what time you received those signals, you could figure out where on the line you were. In fact, if instead of a line, you lived on a piece of paper, you could figure out to one of two points where you were, with the same two points of data.

GPS works with a constellation of many satellites, which broadcast the time on known intervals. If you know exactly where they are (They broadcast this information too, albeit slower), then you can identify exactly where you are, if you know where 3+ of these are and the correct time. With a fourth satellite, you can even tell the time. More just reduces the uncertainty associated with each measurement.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
