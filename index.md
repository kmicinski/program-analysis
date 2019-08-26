---
layout: mainpage
---

## Upcoming deadlines

<ul class="due-list">
{% for post in site.posts %}
    {% capture nowunix %}{{'now' | date: '%s'}}{% endcapture %}
    {% capture duetime %}{{post.due | date: '%s'}}{% endcapture %}
    {% if post.categories contains 'assignment' and duetime > nowunix %}
    <li>
       <span><span class="post-meta"><b>(Due <span itemprop="date">{{ post.due | date: "%b %-d, %Y" }}</span>)</b></span><a class="mainpage-asn-link" href="{{ post.url | absolute_url }}">{{ post.title }}</a></span></li>
   {% endif %}
{% endfor %}
</ul>

## Information

<div class="infomatter">
<table class="infotablestyle">
<tr><td>Course Number</td>
    <td>CMSC 245 (Spring 2019) at <a href="https://www.haverford.edu/computer-science/">Haverford College</a></td>
</tr>
<tr><td>Instructor</td>
    <td><a href="http://kmicinski.com">Kristopher Micinski</a></td>
</tr>
<tr><td>Teaching Assistants</td>
    <td>Jocelyn Dunkley</td>
</tr>
<tr>
    <td></td>
    <td>Myriam Benkoussa</td>
</tr>
<tr>
    <td>Times</td>
    <td>Mon/Wed 12:45-2:15 <i>Lecture</i>  Tu 10:30 / 12:30 <i>Labs</i></td>
</tr>
<tr>
    <td>Office Hours</td>
    <td>Mo/Wed after class and by appointment</td>
</tr>
<tr>
    <td>TA Office Hours</td>
    <td>TBA</td>
</tr>
</table>
<img class="krispic" src="/assets/img/krisbw.jpg">
</div>
    
## Introduction 

Have you ever asked yourself what principles underly programming
languges? How to make an informed decision about which language to
use? Why are some languages apparently faster than others?

These are the kinds of questions we're going to answer in this
class. Together, we'll drill into how the computer executes programs,
gradually pulling apart the complexities involved in turning your
programs from a string of characters to operations performed by your
processor.

To do this, we'll learn languages at three different levels:

- The low level (assembly): how the processor pushes around bits to
  perform the most basic of tasks (arithmetic, moving data, etc..)

- The middle level (C++): how we can leverge low-level niceties (such
  as performance), but retain a structured language so we can scale
  our ideas to large software engineering tasks.

- The high level (Scheme / Racket / Datalog): how we can strategically
  ignore the lower level facilties and focus on the high-level essence
  of the problems we want to solve.

The lower-level the language, the more complexity we'll deal with (in
terms of having to understand what the computer is doing).  So an
auxiliary benefit of this class is that you'll have to learn more
about how computers work. Once we understand what the computer's doing
at a low level, we'll be able to exploit that understanding by writing
highly efficient code. Dually, understanding concepts from
higher-level languages will teach us how to build better
abstractions. We'll even get to the point where we're extending the
languages we use on a day-to-day basis and building new ones.

The goal of this course is to teach you both the nuts and bolts of
languages and to help built intuition about programming paradigms in a
broadly construed manner. When you're done, you still won't know every
language out there. But we hope that you'll be able to thoughtfully
articulate why you choose the language you did, and have enough
intuition to pick up new languages very quickly.

## Course Structure

Please read the [Syllabus]({{ "/syllabus" | absolute_url }}) for course information.
