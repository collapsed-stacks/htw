## Voltage Transformers

- posted by: [EvilPhoenix](https://stackexchange.com/users/-1/78-evilphoenix) on 2011-04-19
- tagged: `electricity`, `science`, `physics`
- score: 3

How does one create an electrical voltage transformer?  What is the science behind why they work?  Are there different types of voltage transformers?


## Answer 104

- posted by: [Pearsonartphoto](https://stackexchange.com/users/-1/67-pearsonartphoto) on 2011-04-19
- score: 3

<p>There are 5 basic kinds of <a href="http://en.wikipedia.org/wiki/Transformer" rel="nofollow">transformers</a>, which I'll try and explain. They are:</p>

<ul>
<li>AC </li>
<li>DC step down</li>
<li>AC to DC</li>
<li>DC to AC</li>
<li>DC step up</li>
</ul>

<p>AC Voltage transformers are essentially pairs of electromagnets, one contained entirely inside the other, which have different winding lengths. The net effect of these dual magnets is that the current coming out from the output line is some multiple of what the input line is, and as power is conserved, the voltage must also be half. A transformer which is not connected to a load will still draw power. These transformations can be lossless, although small losses are common.</p>

<p>DC step down, or more commonly, <a href="http://en.wikipedia.org/wiki/Voltage_divider" rel="nofollow">Voltage dividers</a>, will take the voltage from a higher input source, and step it down to something lower. One of the simplest ways to do so is from a bridge circuit, although more advanced ways work using an op amp. There is an article from <a href="http://www.analog.com/library/analogDialogue/archives/35-02/avoiding/index.html" rel="nofollow">analog Devices</a> which explains how one can be used, including pictures. These transformation involve a small to moderate loss of power.</p>

<p>AC to DC transformation is accomplished usually in 2 steps, listed below. They typically involve significant (~50%) power losses.</p>

<ol>
<li><a href="http://en.wikipedia.org/wiki/Rectifier" rel="nofollow">Rectify</a> the signal</li>
<li>Use a low pass filter on the remaining signal.</li>
</ol>

<p>DC to AC transformation works much the reverse of AC to DC transformation, and are similarly inefficient. Namely, the steps are:</p>

<ol>
<li><a href="http://en.wikipedia.org/wiki/Inverter_%28electrical%29" rel="nofollow">Invert</a> the signal.</li>
<li>Run the signal through a high pass filter, notched at the desired frequency.</li>
</ol>

<p>DC step up transformers typically work in a 3 step process, and are very inefficient. Namely, they:</p>

<ol>
<li>Convert the signal to AC</li>
<li>Step up the AC signal</li>
<li>Convert the signal back to DC.</li>
</ol>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
