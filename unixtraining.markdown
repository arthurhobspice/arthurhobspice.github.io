---
layout: page
title: Unix training
permalink: /unixtraining/
---

I used to teach Unix (Sun Solaris, actually) for three years at Sun Microsystems, being an
instructor for customer and train-the-trainer classes.
Later on, since I was having this experience, I was repeatedly asked to hold Unix training sessions
for my colleagues. For these trainings I compiled some presentation and exercise material.
Feel free to take a look and use - it's mostly simple stuff, but it's the simple things you need
most of the time in an operations or SRE life.

# Unix Fundamentals

This is for absolute beginners who know how to use a (Windows) PC but have never worked on
a Unix/Linux system, or for people who took some first steps on Unix and would now like to
have a systematic walk through all the basics. We concentrace on using the command line (shell)
rather than some GUI tools.

[Seminar slides ](/files/unix_fundamentals.pdf)

# Unix Shell Programming

This one is for people who are familiar with Unix basics and somewhat experienced users of
the command line (shell). Shell programming (aka scripting) can make our lives easier, allowing
to automate many repetitive tasks. Unix commands and controlling key words of the shell are
combined to programming instructions. Shell scripts are typically used in maintenance, operations
or deployment tasks, for setting up and administering Unix systems or for searching and manipulating
large (numbers of) files. Unix/Linux systems come with a lot of executable commands which are
actually scripts, under the hood.

Shell scripts become really powerful when combined with one of the many command line tools
each designed for a specific purpose, for example `grep`, `sed` or `awk`.

[Seminar slides ](/files/unix_shell_programming.pdf)

# Todos

When I find some time, I need to update the courses:

- Concentrate on Linux and, eventually, remove Solaris references
- Concentrate on bash and remove ksh stuff
- Add some pages about the widely used Linux package managers, yum and apt
