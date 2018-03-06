## How does a three-way light switch work?

- posted by: [Josh](https://stackexchange.com/users/-1/20-josh) on 2011-04-18
- tagged: `electricity`, `wiring`
- score: 9

There's a few light switches in my home where two switches control one light: If I turn one light switch on, the light will come on. If I go turn the other lightswitch "on" (putting it in the up position), the light turns off. How does this work? I remember in robotic class many many years ago we were challenged to determine how these worked, and everyone came up with circuit diagrams, all of which were wrong. I've since forgotten the answer!

How do three-way light switches work?


## Answer 41

- posted by: [Stefano Borini](https://stackexchange.com/users/-1/23-stefano-borini) on 2011-04-18
- score: 11

<p>Like this</p>

<pre><code>     [     o-----]-------[--o     ]
     |    /      |       |   \    |
N ---|--o/   A   |       | B  \o--|--- lamp ON ---- AC ~
     |           |       |        |
     [     o-----]-------[---o    ]
</code></pre>

<p>In this case, switches A and B have the light turned on. If you toggle one of them, the light turns off because you remove the neutral from it.</p>

<pre><code>     [     o-----]-------[--o     ]
     |           |       |   \    |
N ---|--o\   A   |       | B  \o--|--- lamp OFF ---- AC ~
     |    \      |       |        |
     [     o-----]-------[---o    ]
</code></pre>

<p>However, if you toggle either the same, or the other one you re-establish the electric contact</p>

<pre><code>     [     o-----]-------[--o     ]
     |           |       |        |
N ---|--o\   A   |       | B  /o--|--- lamp ON ---- AC ~
     |    \      |       |   /    |
     [     o-----]-------[---o    ]
</code></pre>

<p>I consider safer to have neutral on the switch and AC on the lamp, but the opposite choice would work as well.</p>

<p>If you have multiple points, you can use four-way switches, but it may become complex as you have to transport three cables instead of two. An alternative is to use a <a href="http://en.wikipedia.org/wiki/Relay" rel="nofollow">Relay</a> which is simpler but noisier.</p>



## Answer 36

- posted by: [Rory Alsop](https://stackexchange.com/users/-1/49-rory-alsop) on 2011-04-18
- score: 4

<p>This is simple once you know that there are two paths for electricity to travel, and all you are doing with the switches is selecting one or the other. If the two switches are connected to the same wire current flows - effectively the two wires give you 2 out of 4 combinations being on, and 2 being off.</p>

<p><img src="http://i.imgur.com/j2DIN.jpg" alt="3 way switch diagram"></p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
