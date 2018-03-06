## How do CPUs work

- posted by: [Joe](https://stackexchange.com/users/-1/72-joe) on 2011-04-18
- tagged: `computers`, `computer-hardware`
- score: 3

From what I understand about CPUs, they are simply electrical impulses in silicon. How are these signals converted and understood by a computer? Is it something similar to Morse code?


## Answer 124

- posted by: [e.James](https://stackexchange.com/users/-1/54-e-james) on 2011-04-19
- score: 5

<p>A <a href="http://en.wikipedia.org/wiki/Central_processing_unit" rel="nofollow">CPU</a> (Central Processing Unit) is a complex <a href="http://en.wikipedia.org/wiki/Integrated_circuit" rel="nofollow">integrated circuit</a> composed of <a href="http://en.wikipedia.org/wiki/CPU_design" rel="nofollow">many smaller circuits and subsystems</a> which all work together in order to process data and execute instructions. Each of these subsystem is composed of many digital <a href="http://en.wikipedia.org/wiki/Logic_gate" rel="nofollow">logic gates</a>. A modern CPU can contain billions of logic gates.</p>

<p>Digital logic gates are electronic circuits that use an electrical voltage to define simple logical states. A low voltage (typically zero) is used to represent a logical "0", while a higher voltage is used to represent a logical "1". The simplest logic gate is an inverter (<a href="http://en.wikipedia.org/wiki/NOT_gate" rel="nofollow">NOT gate</a>), which takes one logical signal at its input and produces the opposite signal at its output (0 becomes 1 and 1 becomes 0). More complex gates take two or more input signals and produce specific outputs depending on the values of all input signals. Common examples are the <a href="http://en.wikipedia.org/wiki/AND_gate" rel="nofollow">AND gate</a> (which outputs a logical 1 only when <em>all</em> of its inputs are 1) and the <a href="http://en.wikipedia.org/wiki/OR_gate" rel="nofollow">OR gate</a> (which outputs a logical 1 if <em>any</em> of its inputs are 1).</p>

<p>In a typical silicon chip, logic gates are built using <a href="http://en.wikipedia.org/wiki/Transistor" rel="nofollow">transistors</a>, which are essentially tiny switches that use one electrical signal to turn another electrical signal on &amp; off. Modern transistors are <a href="http://en.wikipedia.org/wiki/Semiconductor_device" rel="nofollow">semiconductor devices</a>. In the early days of computing, electrical switching was done using <a href="http://en.wikipedia.org/wiki/Vacuum_tube" rel="nofollow">vacuum tubes</a>. Future CPU designs may use <a href="http://en.wikipedia.org/wiki/Optical_computing" rel="nofollow">light</a> or even <a href="http://en.wikipedia.org/wiki/Organic_computing" rel="nofollow">living cells</a>.</p>

<p>Whatever the technology used to make logic gates, the point is that many small gates can be combined together to perform complex mathematical calculations. In the digital world, numbers are represented in <em>binary</em>, or <a href="http://en.wikipedia.org/wiki/Binary_numeral_system" rel="nofollow">base two</a>. We normally think of numbers in <a href="http://en.wikipedia.org/wiki/Base_%28mathematics%29" rel="nofollow">base ten</a>, which means that you have ten digits ("zero" through "nine") which can be combined to form larger numbers.</p>

<p>In base ten, the number 234 means:</p>

<pre><code>2x(10)^2 (two hundred) +
3x(10)^1 (thirty)      +
4x(10)^0 (four)
</code></pre>

<p>The same number in base 2 would be <code>11101010</code> which means:</p>

<pre><code>1x(2)^7 +
1x(2)^6 +
1x(2)^5 +
0x(2)^4 +
1x(2)^3 +
0x(2)^2 +
1x(2)^1 +
0x(2)^0
</code></pre>

<p>Binary digits are usually called <a href="http://en.wikipedia.org/wiki/Bit" rel="nofollow">bits</a>. Eight bits can be used to represent any number between 0 (<code>00000000</code>) and 255 (<code>11111111</code>). Eight bits are usually called a <a href="http://en.wikipedia.org/wiki/Byte" rel="nofollow">byte</a>, and most CPUs deal with numbers that are two, four, or eight bytes long (16-bit, 32-bit, or 64-bit <a href="http://en.wikipedia.org/wiki/Computer_architecture" rel="nofollow">architecture</a>).</p>

<p>Every CPU has its own "language" which we call <a href="http://en.wikipedia.org/wiki/Machine_code" rel="nofollow">machine code</a>. This "language" uses binary numbers to represent <a href="http://en.wikipedia.org/wiki/Instruction_set" rel="nofollow">instructions</a> that can be performed by the CPU. Regardless of the specific <a href="http://en.wikipedia.org/wiki/Programming_language" rel="nofollow">programming language</a> used, the end result is always machine code running on the CPU.</p>



## Answer 235

- posted by: [bcsanches](https://stackexchange.com/users/-1/17-bcsanches) on 2011-04-20
- score: 1

A good text about CPUs that might help: http://www.lighterra.com/papers/modernmicroprocessors/

This article discuss how modern CPUs do their work and specially how the CPU pipeline works, also includes an interesting section explaining why not only megahertz define the CPU speed.


## Answer 79

- posted by: [Ward](https://stackexchange.com/users/-1/36-ward) on 2011-04-18
- score: 0

The idea of it being like Morris code isnt to far of a stretch. The signals actually are sent as binary ( 1 or 0 ). 1 Being on and 0 being off. The basic manipulation of these signals are the fundamental aspects of computing as far as the electrical impulses are concerned. This information is then manipulated through a series of IC(integrated circuits) and via the intricate use of logic gates.


## Answer 121

- posted by: [Pearsonartphoto](https://stackexchange.com/users/-1/67-pearsonartphoto) on 2011-04-19
- score: 0

<p>The basic building blocks of a computer are the and, or, and not gates. They work as follows:</p>

<ul>
<li>And= Returns 1 if both inputs are 1</li>
<li>Or= Returns 1 if either or both inputs are 1</li>
<li>Not= Returns the opposite of what signal is input.</li>
</ul>

<p>To make a rather complex problem simpler, basically a computer will pattern match the input code, and given that code, will execute an appropriate operation. Operations can include putting data into a memory location, adding two pieces of data, performing and/or/not operations, bit shifting, and other fun stuff too. Feel free to ask more questions, or take a look at <a href="http://www.howstuffworks.com/microprocessor.htm" rel="nofollow">this article</a>.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
