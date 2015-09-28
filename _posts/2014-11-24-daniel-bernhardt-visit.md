---
layout: post
title: Daniel Bernhardt Visit
categories:
- Daniel Bernhardt
- Facebook
- spelling
- edit distance
- hash table
---

Daniel is visiting from Facebook London where he’s been working for just
over a year. Before that he worked for 4 years at Microsoft Search, and
previous to that he did his PhD in applied machine learning for
emotional gesture recognition and his Undergraduate in Computer Science
(both at the University of Cambridge).

Daniel Bernhardt visit. We will learn about how Facebook deal with the
challenge of spell correction for the vast range of names that exist.
Daniel will give us a talk followed by a Q&A about anything you care to
have answered!

Daniel spoke about the spell checking problem, two different types of
spelling errors cognitive errors and typo errors, and how these are
passed into the search engine. Search engine queries take several
hundred milliseconds. Your typed query is passed to the search engine
after spell checking.

“A System for searching the social Graph” (VLDB 2013)

### First Approach

We talked about the [*edit
distance*](http://en.wikipedia.org/wiki/Edit_distance) as a way of
comparing correct names (in a dictionary) to incorrect names. This is a
dynamic programming approach for computing the distance of the query
from a ‘correct’ query.

Through a [*hash table*](http://en.wikipedia.org/wiki/Hash_table) you
can compute look ups quickly.

In practice the dictionary could be really massive! 1 billion user
nodes, 240 billion photo nodes, 1.2 trillion posts, 1 trillion edges.

To build a dictionary of unique names: there are 73 million unique first
name and 67 million unique surnames. 560,800,810 unique en-us names! The
dictionary would be very large and nearly 40% of US full names are
unique!

Context also needs to be included, you are often spelling friends names,
you don’t want the average of all names!

Edit distances also don’t encode properly mistakes that are more likely
(for example due to a keyboard layout).

### Actual Approach

Language model takes any given sequence and gives a probability
associated. n-gram models can be used for modelling language.

We talked about error models and how they can be derived from query
rewrites. This is when a user types a search and then doesn’t seem to
select any of the returned results. They then change the query and that
new query gives the right result. This gives a lot of valuable
information about what the original query should have been.

We talked about challenges including doing different languages, and
making general solutions. In particular we talked about the challenge of
*domain adaptation* and how a spell checker for one particular domain
may not be appropriate for another domain. We talked about the
importance of data and feedback.

Daniel talked about how widely machine learning is used across the site,
and how, often, it’s not the learning algorithm itself that’s a problem,
but evaluating the quality of the model or extracting the data for
learning.

Charles asked about when the system is finished, Daniel said broadly
speaking that they are always looking for continuous improvement. Whilst
the target is to focus on impact, they don’t consider a system done, but
if the system is working well, then they may reprioritise on something
else.


** Also Non Academic Task 4 **


Non-Academic 4
--------------

Read through the[*Computer Science First Year’s Tutorial
Booklet*](http://www.dcs.shef.ac.uk/intranet/teaching/public/tutorials/level1/firstyeartutorials.pdf)
on *exam skills*. Read old exam papers and think about what the
question’s aims are. How to DCS and SoMaS differ in their exam question
style? How are they similar?

