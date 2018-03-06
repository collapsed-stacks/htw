## How do CD readers (CD players) work?

- posted by: [EvilPhoenix](https://stackexchange.com/users/-1/78-evilphoenix) on 2011-04-18
- tagged: `electronics`
- score: 3

How do CD players operate?  How do they get the data from the CD, and how do they convert that into readable data that speakers/headphones/audio output devices can understand?


## Answer 117

- posted by: [Pearsonartphoto](https://stackexchange.com/users/-1/67-pearsonartphoto) on 2011-04-19
- score: 4

I'm going to explain first how a data CD is read, and then how a CD is read.

A data CD consists of a series of bumps in a groove pattern. These bumps are all the same size, and are invisible to the human eye. A laser shines on the correct location of the potential bump. If it is scattered, then a bump was there, if it's reflected, there was no bump. This is a single data point of 1 or 0.

CDs are organized into several sections. A data CD has some error checking included, while most audio CDs do not. I won't bore you with the details, but I will say that is is organized. 

In essence, the way that a data CD works is almost identical to an audio, with the main difference being what happens after the data is read, and the removal of some error checking. The data on a CD is such that a given amount of space on the CD corresponds to 1 second of data. Actually, every two bytes is 1/44100th of a second. The signal corresponds to an analog value, which can be achieved using a Digital to Analog converter. The signal is played at this constant rate, reproducing the original signal.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
