Who needs scripts?
==================
I just found myself in a situation where I wanted to rename files according
to a pattern.

Usually, I ignore the task or do it manually.
It's too bothersome to invest so much thought into learning how to do it,
even though it should be a simple job.

This time, I decided to at least do a quick search.

Suggestions
===========
Stackoverflow et al proposes sollutions involving:
 
 - awk
 - find -exec
 - python
 - rename
 - shell scripts

Problem with existing tools
===========================
 - Shell scrips have cluttered syntax.
 - A WHOLE interpreted language just for browsing files and executing commands?
 - General purpose scripting languages might be too much for simple scripts.
 - Programs such as rename are to specific. I prefer unix philosophy.
 - I don't like interactive modes of languages.

Problem with alternatives
=========================
Bash redirecting is powerfull.
One might separate it into dedicated tools, but the syntax overhead is too big.

Having e.g. for loops at command prompt is powerfull.
One could write a script?
Or launch an interpreter dedicated for interactive mode when such is needed.
A dedicated loop program, would break every standard.

What syntax should be adopted/created?

Solution
========
I have no concrete solution.

Should not have to import file capabilities.
Management of files should be its priority.

The loops, redirection and such could be sent as arguments to a program.
That way, usage is unchanged except for a prefixed word.

One program, e.g. cli, could be for cd'ing around and executing commands.
Another, e.g. itrp, could interpret scripts from stdin, file or args.
