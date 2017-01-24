Freeing memory on exit
======================
If you *alloc, you free.
That one's obvious.
One should always avoid memory leaks.

The question is whether or not to free upon program termination.

As I tried to find answers, I noticed they were all conflicting.
At the same time, different opinions where held.
Because of that, I will try to compile some of the arguments pro and con.

Pros of freeing
===============
Do it as good practice
----------------------
Even though the OS cleans up, it is good exercice to clean.

It serves as debugging
----------------------
Maybe you catch some bugs and leaks when you try to free.

Use memorychecking tools
------------------------
If you use e.g. valgrind, it will give obstructive warnings.

> If you don’t care about using error-detection tools like valgrind,
> then you don’t care about writing good programs.

Code reuse
----------
Someone might reuse your code inside another program.

Embedded systems
----------------
There might not be any OS or memory manager.
Relying on the OS is "bad practice".

It should be easy
-----------------
With release strategies e.g. a memory pool.

The OS doesn't handle everything
--------------------------------
Temporary files and external resources is NOT cleaned by the OS.
This cleanup is elegantly combined with freeing.

Cons of freeing
===============
The OS is faster
----------------
The OS just purges everything, whereas you might have to traverse lists, etc.
If you have alloced a lot, the OS obliterates it blazingly swift.

It's simpler and cleaner
------------------------
Your cleanup code will only do the essentials.

It's unnecessary
----------------
Do you clean your trash before throwing it out?

New bugs
--------
The OS does it right, you might fuck it up and make it worse.

Conclusion
==========
Allthough there are many arguments pro, the cons might still outway them.
I am unable to determine the optimal solution.
