## How does a master key work?

- posted by: [Slipstream](https://stackexchange.com/users/-1/39-slipstream) on 2011-04-21
- tagged: `mechanics`, `locks`
- score: 11

How does a lock work, so that not only the right key can open in but also a different 'master' key, which can open several locks?


## Answer 320

- posted by: [Brad](https://stackexchange.com/users/-1/59-brad) on 2011-04-21
- score: 13

Well, this gets kind of deep into how pin tumbler locks work in the first place.

**LOCKS**

Every key has a series of bumps and valleys.  You can see that the peaks are somewhat haphazard, but the valleys are flat and precise.  Inside the lock, there are a series of (usually 4-7) stacks tiny metal cylinders which travel vertically.  These are called pins.  The pins fit into the valleys in your key.  Each pin is very roughly the diameter of a grain of rice, with a length of 2-8mm or so.  The pins are on springs so that they are normally pushed down, but when the key is inserted, the pins are raised up.  When they are all raised to the precisely correct level, the lock is allowed to turn.

In a normal lock, each stack of pins has two pins.  The one that touches the key is called the key pin.  When the tiny gap between the pins is raised to the "shear line" of the lock, that stack does not prevent the lock from turning.  When every stack is raised to the correct level, the lock can be opened.

**MASTER KEYED LOCKS**

In a master key system, the stacks have more than two pins.  As such, more than one valley height is acceptable for each position along the key.

If you had the following set of 4-pin locks (I am using [x,y] to mean a pin stack that can be opened by a key cut to either x or y at that location):

    [1,2] [1,5] [1,8] [1,4]
    [1,3] [1,3] [1,3] [1,3]
    [1,6] [1,6] [1,6] [1,6]

You can see that the 1111 key opens all three locks, and the keys 2584, 3333, and 6666 are the "change keys".

**That's it** - what follows is merely hobby. :)

A 9 represents the deepest cut, and a 0 or 1 is the shallowest cut.  The master key is usually set up to use lower numbers; this prevents a user from filing down his change key into a master key.

(It is interesting to note that there are actually 16 keys that open each of these locks...)

There are other systems you can use too.  For example if we modify the first stack of the above three locks

    [1,2] [1,5] [1,8] [1,4]
    [1,2] [1,3] [1,3] [1,3]
    [1,2] [1,6] [1,6] [1,6]

We can see that 2111 is still a master key for these locks.  This allows multiple levels of security.  For example these three locks could be server closets, and you could give the building sysadmin the 2111 key.  However, you could give the head of facilities the 1111 key which would open every door in the building.

This is great because it allows you to have cascaded security systems without needing more than 2 levels in any stack.  The more levels, the more expensive the lock is to produce and maintain, and the easier it is to pick (imagine if every level was a valid level...)

Also cheaper to build is a system like this.

    [1] [1] [1] [1,4]
    [1] [1] [1] [1,3]
    [1] [1] [1] [1,6]

If you have every worked/lived in a master-keyed system, you may find that the first section of your key (near the hilt) is the same as your coworkers/dorm-mates.


## Answer 313

- posted by: [ursa_arcadius](https://stackexchange.com/users/-1/68-ursa-arcadius) on 2011-04-21
- score: -2

<p><a href="http://home.howstuffworks.com/home-improvement/household-safety/security/question710.htm" rel="nofollow">This article</a> on HowStuffWorks provides an excellent explanation.  It essentially has to do with how the key is shaped.  A key that opens only one door is similar to a master key, but different enough that it can not open all the doors.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
