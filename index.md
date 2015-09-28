---
layout: page
tagline: Tutorials at Interface of CS and Maths
---

The interface between Computer Science and Mathematics is at the heart of the data science revolution. Historically there has been a different cultural approach to the way Mathematics and Computer Science are taught at University level. These tutorials are about 'bringing it together'. They are small group sessions targeted at discussing the interface between Computer Science and Mathematics and emphasizing its importance in scientific computing and data analysis.

## Your Personal Tutor

You also have a personal tutor, that means if you are having problems
with the course, life, the universe or anything, I’m your main contact.
Feel free to catch me after our meetings if you’d like to arrange an
appointment, or drop me an email. Unfortunately, I do get a lot of email
and I do sometimes miss things. So if you don’t get a reply, feel free
to pester me again.

If something particularly serious happens and you
need to inform us you can also make contact with Zoe Fletcher, who is
our administrator for Computer Science in charge of all things teaching.
She’s really great, and knows all the program rules. Or Amanda Sharkey
(1st year tutor for Computer Science).

Late in the first semester we will try and organise times for individual
meetings.

## Non Academic Tasks

We want these meetings to be about the academic side of life, they are
not assessed, but it is a chance for us to all talk about interesting
things in maths and computer science. However, we also need to cover some non-academic material. Different tasks are scattered through the tutorials.



# Tutorials

<ul class="post-list">
    {% for post in site.posts %}
      <li>
        <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>

        <h2>
          <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
        </h2>
      </li>
    {% endfor %}
  </ul>


