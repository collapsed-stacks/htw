## How does Hyper Threading work?

- posted by: [Jacob](https://stackexchange.com/users/-1/28-jacob) on 2011-04-18
- tagged: `electronics`, `computers`, `hyperthreading`
- score: 9

I've noticed some of my servers have Hyper Threading on the Intel CPUs, I've always wondered what it is, and how it works?


## Answer 142

- posted by: [starblue](https://stackexchange.com/users/-1/107-starblue) on 2011-04-19
- score: 8

<p>A processing core in a large modern CPU has many functional units that can do various operations, from simple addition to floating-point operations. The machine instructions are not executed in a fixed sequence but scheduled on units according to their availability.</p>

<p>A single <a href="http://en.wikipedia.org/wiki/Thread_%28computer_science%29" rel="nofollow">thread</a> of execution typically uses only some part of the available execution units, and the rest of them would be idle. Hyperthreading allows more threads to compete for the execution units within the core, so that more of them are being utilised at any given point in time.</p>

<p>Depending on the characteristics of the threads they may get along well and not hinder each other much--in this case the total work done is almost doubled. In other cases the two threads may compete for the same scarce resources and get less done than a single thread would in the same time.</p>



## Answer 76

- posted by: [ursa_arcadius](https://stackexchange.com/users/-1/68-ursa-arcadius) on 2011-04-18
- score: 2

A very simple answer, the CPU trades off on two "threads" so it is essentially working on two different things in each core.  Here is a great article about it: http://www.makeuseof.com/tag/hyperthreading-technology-explained/



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
