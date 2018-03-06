## How does the "Abacus" work?

- posted by: [MalsR](https://stackexchange.com/users/-1/31-malsr) on 2011-04-18
- tagged: `abacus`, `calculation`, `mathematics`
- score: 5

A handheld calculating aid that has been around for a long time. A common abacus consists of a grid in a wooden frame. How does the upper rows and lower rows aid when performing calculations?... how does it work?


## Answer 123

- posted by: [DTing](https://stackexchange.com/users/-1/62-dting) on 2011-04-19
- score: 5

<p>There are a couple different types of abacus but the basics are pretty simple:</p>

<pre><code>10000's   1000's    100's     10's      1's
      O        O        O        O        O        Heaven Beads
      |        |        |        |        |
    ========================================
      |        |        |        |        |
      O        O        O        O        O        Earth Beads
      O        O        O        O        O
      O        O        O        O        O
      O        O        O        O        O
</code></pre>

<p>The Basics:</p>

<p>Representation the numbers 0 - 9 (rotated to right for easier typing)</p>

<pre><code>0:  OOOO-|-O
1:  OOO-O|-O
2:  OO-OO|-O
3:  O-OOO|-O
4:  -OOOO|-O
5:  OOOO-|O-
6:  OOO-O|O-
7:  OO-OO|O-
8:  O-OOO|O-
9:  -OOOO|O-
   earth | heaven
</code></pre>

<p>Representing numbers: Split the number up by digit and represent those numbers in appropriate columns:</p>

<p>examples:</p>

<pre><code>27:
10    OO-OO|-O
 1    OO-OO|O-

4589:
1000  -OOOO|-O
 100  OOOO-|O-
  10  O-OOO|O-
   1  -OOOO|O-
</code></pre>

<p>Addition:</p>

<p>Register starting number then add beads from right to left:</p>

<p>example:</p>

<pre><code>999 + 75
</code></pre>

<p>register:</p>

<pre><code>100  -OOOO|O-     9
 10  -OOOO|O-     9
  1  -OOOO|O-     9
</code></pre>

<p>adding 1's digit:</p>

<pre><code>1000  OOO-O|-O    1
 100  OOOO-|-O    0
  10  OOOO-|-O    0
   1  -OOOO|-O    4
</code></pre>

<p>adding 10's digit:</p>

<pre><code>1000  OOO-O|-O    1
 100  OOOO-|-O    0
  10  OO-OO|O-    7
   1  -OOOO|-O    4
</code></pre>

<p>Subtraction:</p>

<p>Register the starting number and then subtract starting from left to right.</p>

<p>example:</p>

<pre><code>1452 - 723
</code></pre>

<p>register:</p>

<pre><code>1000  OOO-O|-O    1
 100  -OOOO|-O    4
  10  OOOO-|O-    5
   1  OO-OO|-O    2
</code></pre>

<p>subtract 100's digit. Because the number we are subtracting is larger than the number in the column, we go left one column and subtract one unit, then add the difference of 10 and the number we are subtracting: 10-7 = 3</p>

<pre><code>1000  OOOO-|-O    0    (1 subtracted)
 100  OO-OO|O-    7    (3 added)
  10  OOOO-|O-    5
   1  OO-OO|-O    2
</code></pre>

<p>subtract 10's digit.  </p>

<pre><code>1000  OOOO-|-O    0    
 100  OO-OO|O-    7 
  10  O-OOO|-O    3
   1  OO-OO|-O    2
</code></pre>

<p>subtract the 1's digit. Same as before, 10's digit remove a unit, add 10-3 to the 1's column.</p>

<pre><code>1000  OOOO-|-O    0    
 100  OO-OO|O-    7 
  10  OO-OO|-O    2    (1 subtracted)
   1  -OOOO|O-    9    (7 added)
</code></pre>

<p>Multiplication and Division take a bit longer to explain, so you can read about them online or try to decipher <a href="http://www.youtube.com/watch?v=ouSxC-hJL4I" rel="nofollow"><strong><code>this</code></strong></a> video (warning, guy is talking very fast).</p>

<p><a href="http://www.tux.org/~bagleyd/java/AbacusAppJS.html" rel="nofollow"><strong><code>Here</code></strong></a> is an online abacus to play with.</p>



## Answer 82

- posted by: [Ward](https://stackexchange.com/users/-1/36-ward) on 2011-04-18
- score: 1

<p><img src="http://i.imgur.com/ghXqO.jpg" alt="enter image description here"></p>

<p>its hard to tell in the picture but basically the beads in the upper level come in rows of one or two and are worth 5x the base value of the bottom column its above, as thus both beads being set is equal to one bead in the next bottom column being set as you would carry the number over for being greater than 9, 10 in this case.</p>

<p>The bottom row of beads starting on the right are all worth 1 the bead in the top row above it being worth 5.
The second column of the bottom row is in tenths so its beads would be each worth 10 with the top bead being worth 50.</p>

<p>the beads are slid either from the top row or the bottom toward that middle seperator right to left.</p>

<p>The bottom being refered to as the earth beads and the top being refered to as heaven beads.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
