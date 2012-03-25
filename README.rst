========================
Advanced Security Topics
========================

This repo contains the slides from my talk on Advanced Security at
Pycon US 2012.

https://us.pycon.org/2012/schedule/presentation/467/

I strongly encourage you to ask me questions about the material
covered in this presentation. I'm usually on IRC on the freenode
network (PaulM), and respond pretty quickly via twitter
(@paulrmcmillan) or email (paul@mcmillan.ws).

The video:

* http://www.youtube.com/watch?v=JOXwclgvXB0
* http://pyvideo.org/video/638/advanced-security-topics

Brian Rue's Notes:

* http://brianrue.wordpress.com/2012/03/09/pycon-2012-notes-advanced-security-topics/

March 9th 1:45 p.m. – 2:40 p.m.

Description
===========

If your Python application has users, you should be worried about
security. This talk will cover advanced material, highlighting common
mistakes. Topics will include hashing and salts, timing attacks,
serialization, and much more. Expect eye opening demos, and an urge to
go fix your code right away.

Abstract
========

If your Python application has users (even if it's used offline), you
should be worried about security. This talk will cover advanced
material, highlighting common mistakes.

Hashing and encryption can be tricky to get right. We'll discuss when
to use hashing to sign data, and how to choose the right encryption
algorithm (spoiler: don't). We'll demonstrate length extension
attacks, and discuss how to prevent them.

Another common mistake is the incorrect use of pseudo-random number
generators. We'll discuss the fix, and some of the dangers associated
with it.

Timing attacks are relatively exotic, but as applications move into
shared data centers (and shared virtual machines) they have become
easier to implement and more dangerous. They're a very common class of
bugs, but fixing them (and proving they're fixed) can be difficult.

Pickle is a common and easy to use serialization format for Python
objects. Unfortunately, it's also insecure when attackers can send or
modify the pickled data. We'll discuss strategies for signing pickled
objects, and alternate serialization formats.

The final portion of the talk will discuss a meta security problem
within the Python community. I'll be demonstrating live code that can
compromise even the most locked down of servers, and discussing the
steps we need to take as a community to mitigate this threat moving
forward.
