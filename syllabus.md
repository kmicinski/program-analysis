---
title: Syllabus
layout: page
---

## Principles of Programming Languages
(*CMSC 245* at Haverford College)

**Note**: parts of this syllabus are subject to change with adequate
notice to students.

An introduction to the design and implementation of programming
languages, including lab experience using different kinds of languages
and experience implementing programming language features.

**Prerequisites**:
  - CMSC 106 or 107 (or 206 at Bryn Mawr) or permission from instructor

**Workload**:
  - 3 lecture hours per week
  - 1 lab hour per week
  - This will be a lab / project intensive class. Approximately 6-10
    hours per week *outside* of class will be expected from
    students. I recommend against taking this course concurrent with
    other project-heavy courses.

**Cap**: 24 (Hard cap due to room size)

## Course Overview

This course will introduce many of the principles of programming
language design and implementation. We will discuss numerous features
of several programming languages and the algorithms and data
structures that are needed to provide these features. Labs and
homework will cover both the use of various features and high-level
understanding the algorithms and data structures involved in their
implementation. CMSC 350--Compiler Design--provides more in-depth
information about many of these algorithms and data structures through
labs covering their application to a single simple language.

CMSC 245 lectures (and labs) will include examples (and exercises) in
C++, Racket, and x86 or LLVM assembly language. No prior knowledge of
C++, Scheme, assembly is needed for this course, but students should
be familiar with the programming techniques from CMSC 105/106
(e.g. creation of classes and functions/methods in Python (or some
other language), and confidence with basic uses of both the pure
functional and imperative views of functions and data).


## Grading

- Projects: 50%
- Labs: 10%
- Exams: 35%
  - Midterm 1: 17.5%
  - Midterm 2: 17.5%
  - This course will not have a final exam
- Participation: 5%
 - Participation will *not* be "free" and will be measured in various ways (including the autograder)

Note that both midterms 1 and 2 may include a programming aspect where
live programming is required. I reserve the right to make the midterms
"coding exams." You should expect that exams will include both written
and programming components.

## Autograder

Projects in this course will be graded by an automatic grader. We may
adjust projects so that portions of the projects include style-based
grading, though we will *not* employ subjective grading. More
pointedly: we will *not* award partial credit for solutions that have
the right ideas but do not pass our tests.

You will email me at the beginning of the class to get your username
and password for the autograder.

## Late Projects and Extensions

I used to extend project deadlines, but I have found that this is
often unfair to the students who start on time (and more students than
I would have thought have raised this point to me
privately). Therefore, project extensions will be rare--and usually
only done if it is becasue of a mistake I made. Project extensions for
students will not be granted except for religious observances and
extenuating circumstances (family illness, etc..). The late policy is
as follows:

- Projects turned in on time will earn a maximum of 100%

- Projects turned in up to 48 hours late will have a 15% penalty
  applied.

- Projects turned in after 48 hours late (until the end of the term)
  will have a 30% penalty applied.

- Your project grade always be the maximum possible. For example,
  let's say you make an on-time project submission for 60%, but you
  then turn in a project which earns an 75%. This submission would
  earn a 63.75%. Three days after the deadline you turn in a project
  earning 100%. Your final score is 70%, as the 70% (100% with a 30%
  penalty) still got the maximum grade of any submission.

In other words, you *should* be able to earn **at least** a 70% on all
of the projects with enough work.

## Texts

All the books for this course are free with the exception of "The C++
Tour." I will disseminate copies of the relevant C++ Tour chapters,
and there are a few free chapters online.

- [The C++ Tour](https://isocpp.org/tour) First four chapters
  available for free.

- [Shriram Krishnamurti's free book "Programming languages: Application and
  Interpretation"](http://cs.brown.edu/courses/cs173/2012/book/book.pdf)

- [The Racket Guide](https://docs.racket-lang.org/guide/)

- [The C++ Programming
  Language](https://www.amazon.com/C-Programming-Language-4th/dp/0321563840). This
  is a reference book. I don't think it's worth buying yet, since it
  includes a lot of material irrelevant to the class. But if you want
  to become an expert-level C++ programmer it might be useful to pick
  up a copy.

## Topics

We​ ​will​ ​cover​ ​parts​ ​of​ ​the​ ​following​ ​topics,​ ​adjusted​ ​for​ ​time​ ​and​
​pace​ ​of​ ​the​ ​course,​ ​along​ ​with student​ ​interest​ ​in​ ​each​ ​area.

- C++: Intro and Syntax
  - Loops, pointers, structs, classes, etc...
- Virtual Method Tables
- RAII
- x86 Assembly Programming
  - Calling conventions
  - Data sections
  - Binary layout
- Low-level security / exploits
  - Buffer overflows / attack injection
- Lambda Calculus
- Racket
  - S-Expressions, Immutability, etc...
- Higher-Order Functions
  - Map, fold, SKI calculus, etc..
- Formal Language Semantics
  - Big-Step Semantics
  - Small-Step Semantics
- Church-Encodings
- Continuations, call/cc, exceptions, delimited continuations, etc..
- Closures
- Interpreter implementation:
  - Stack passing
- CPS Conversion
- Type Systems
  - Typed Racket
- Logic Programming
- Datalog

## Projects and Labs

This course will have between six and eight individual projects and
(roughly) weekly labs. Each of these will be completed using the
course's autograder. Lab attendance is expected and required. You may
be excused from labs with adequate notice to and permission from the
instructor.

## Collaboration and the Honor Code

The [CS Collaboration
Policy](https://docs.google.com/document/d/1xpnhkXiqiQuktb_p8NkFKm-uhRCNoIYTeZPZTFLDIt4/edit?usp=sharing)
will govern work in this course; as the semester progresses, we will
add detail about what at-the-computer help is acceptable for this
course. For now, the big ideas are:

- Read and understand the policy

- You should feel free to discuss "ideas" about the solution with
  peers, but you should basically never be getting help from peers
  about your code. If you do, it should only be in the abstract (e.g.,
  "can you use operator overloading to implement that?" or "do you
  think it would be sensible to implement this with `map`?") and not
  particularized to your codebase.

- Cite all help other than the professor, T.A., and
  required/recommended text (you are allowed to cite those if you
  wish, but it is not required unless you are specifically told
  otherwise); note that proper citation is sufficient to avoid any
  charge of academic dishonesty, and we will not be particularly
  focused on copyright law during lab work.

- It is fine to get help away from the computer, as long as you erase
  all notes and return to your computer with only the new
  understanding in your head.

**Most importantly**: You should **never** share code with another
  student. This includes both sending a file to another student and
  "over the shoulder" copying (even when, e.g., variable names are
  changed, etc..). In the eyes of the instructor, these are both
  equally bad. This bears repeating: you should never be sitting and
  helping another along by writing their code. By doing so you are
  both violating the honor policy and disadvanting the student you are
  helping (as they may not then properly learn the material).

## ADS and Student Support

Haverford College is committed to providing equal access to students
with a disability.  If you have (or think you have) a learning
difference or disability – including mental health, medical, or
physical impairment, please contact the Office of Access and
Disability Services (ADS) at `hc-ads@haverford.edu`. The Coordinator
will confidentially discuss the process to establish reasonable
accommodations.

Students who have already been approved to receive academic
accommodations and want to use their accommodations in this course
should share their verification letter with me and also make
arrangements to meet with me as soon as possible to discuss their the
specific accommodations. Please note that accommodations are not
retroactive and require advance notice to implement.

It is a state law in Pennsylvania that individuals must be given
advance notice if they are to be recorded. Therefore, any student who
has a disability-related need to audio record this class must first be
approved for this accommodation from the Coordinator of Access and
Disability Services and then must speak with me. Other class members
will need to be aware that this class may be recorded.

## Slack

Slack is an instant messaging app for teams. We'll be using it,
hopefully a lot. This is the best place to get in touch with me for
one-off questions, ask for an appointment for office hours,
etc.. Please join the course Slack by clicking this link:

[Join here!](https://join.slack.com/t/cs245-s19/shared_invite/enQtNTI4MDMwMDE1NDkyLTMzNzY5NTZjZWRlZDNkZTczY2Y0YzQ1NGNhMGE3MzIwYjUxNzA5NTIzYmI0Zjc5ODY2NTg3Njg3N2RmMDE2YmQ)

## Computer Configuration and the Autograder

The following tutorial explains how to set up 

https://www.youtube.com/watch?v=w7wLvLb2qCw

