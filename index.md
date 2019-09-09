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
    <td>CIS 700 (Fall 2019) at <a href="http://eng-cs.syr.edu/our-departments/electrical-engineering-and-computer-science/">Syracuse University</a></td>
</tr>
<tr><td>Instructor</td>
    <td><a href="http://kmicinski.com">Kristopher Micinski</a></td>
</tr>
<tr>
    <td>Times</td>
    <td>Mon/Wed 3:45-5:15 <i>Lecture</i></td>
</tr>
<tr>
    <td>Office Hours</td>
    <td>Thursdays, 10:30AM-11:30AM</td>
</tr>
</table>
<img class="krispic" src="/assets/img/krisbw.jpg">
</div>
    
## Introduction 

Program analyses answer questions about the behavior of programs. For
example, a control-flow analysis for an object-oriented language could
be used to answer the question: at a given (polymorphic) method
invocation, which method(s) may be invoked? Such analyses power
compiler optimizations which replace the (comparatively) expensive
indirect method invocation with a cheaper direct call.  Critically,
program analyses reason about all possible program behaviors in order
to make such optimizations safely. While this seemingly violates the
halting problem, program analysis tools gain decidability by making
approximations: the analysis must occasionally give imprecise results
to soundly reason about all possible executions.

This course will teach students how to systematically build, apply,
and evaluate program analyses in a wide variety of languages and
paradigms (functional, imperative, relational, etc...). We will begin
by studying the foundations of formal language semantics. To help
ground this theory in practice, students will implement interpreters
for several core programming languages (core Scheme, Featherweight
Java, etc...).  Then, we will move on to building “abstract”
interpreters, which execute programs not with concrete inputs (e.g.,
the number 5) but instead special abstract values which approximate a
(possibly infinite) set of concrete values (e.g., the set of positive
integers). This allows us to generalize a program’s behavior on all
possible inputs.

All program analyses must at some point approximate program
behavior. For example, one (useless but correct) analysis might simply
say “every function could return every possible value if it terminates
at all.” Clearly, this would not be a very useful analysis, so
analysis designers must balance analysis precision with analysis
complexity. A focus of the course will be to teach students the
primary axes of analysis sensitivity (e.g., call sensitivity, object
sensitivity) and help understand the ramifications of language
features (e.g., classes, higher-order functions, etc…) on analysis
performance.

Logistically, the course will involve several individual projects
implementing and evaluating program analyses on several prototypical
languages (e.g., core Scheme), alongside a more ambitious capstone
project that engineers an analysis for a larger language (such as
Java).

## Course Structure

Please read the [Syllabus]({{ "/syllabus" | absolute_url }}) for course information.
