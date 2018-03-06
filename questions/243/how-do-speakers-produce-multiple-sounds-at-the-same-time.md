## How do speakers produce multiple sounds at the same time?

- posted by: [ursa_arcadius](https://stackexchange.com/users/-1/68-ursa-arcadius) on 2011-04-20
- tagged: `music`, `sound`, `hearing`
- score: 2

When listening to music sometimes the parts are so complex and layered that it seem it would be impossible to combine all those sounds into one sound wave.  When listening to them live I would imagine that you are just hearing the combinations of all the different sound waves from the various instruments but in recorded media they have to be created from one source. How are they all reproduced so clearly?


## Answer 251

- posted by: [Pearsonartphoto](https://stackexchange.com/users/-1/67-pearsonartphoto) on 2011-04-20
- score: 3

Any one-dimensional signal can be represented by some sort of a plot. One can analyze this plot, to determine the frequencies which are represented over any given window. 

For instance, if there are two piano notes being played at the same time, and no other signal/noise, then the frequency of these two notes will be represented by two spikes in the frequency transformation. Humans can tell that there are two different notes, as can a computer.

But, in order to tell that there is multiple notes being played, a transform has to occur of the input signal. In order to reproduce the sound, all that needs to be done is to pass the input signal to the speaker, which will imitate the signal as received by the original microphone at a given time.

Now, some speakers are better at representing one range of frequencies better than others. For instance, sub-woofer is much better at representing low frequency sounds than a tweeter. It is common for a smart system to know this, and to pass only the frequencies which can be reproduced by the appropriate speaker.


## Answer 336

- posted by: [whatsisname](https://stackexchange.com/users/-1/137-whatsisname) on 2011-04-22
- score: 2

<p>It's all because of the math involved.</p>

<p>All repeating waveforms can be represented as the sum of a series of sin waves at all frequencies with varying amplitudes. </p>

<p><a href="http://en.wikipedia.org/wiki/Fourier_transform%20%22Fourier%20Transform" rel="nofollow">A Fourier Transform</a> is the mathematic operation that takes the signal, and goes back to find the amplitude of the sin waves building up the original signal. You've probably seen a spectrum analzer on some stereos:
<img src="http://i.imgur.com/IXTbL.jpg" alt="enter image description here"></p>

<p>That is a graphic visualization of the average amplitude for bands of frequency, that graphic is made by doing the Fourier Transom of the music being played. If you did nothing but play a single note on a violin, you would have a singe very high peak centered at the frequency of the note you are playing, and smaller ever decreasing spikes at integer multiples of the original frequency (harmonics).</p>

<p>And, so lastly, our brains have wiring that perform the Fourier transform, and they do it extraordinarily well. They break the signal out into it's component parts and do processing on it, and that is what allows you to hear a C, E, and G simultaneously in a C major chord.</p>

<p>And if your spectrum analyzer had every band at the same level, you'd have <a href="http://en.wikipedia.org/wiki/White_noise" rel="nofollow">White noise</a></p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
