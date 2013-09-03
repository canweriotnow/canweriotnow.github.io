---
layout: post
title: "Teaching Kids to Code: We're Doing It All Wrong"
date: 2013-08-06 21:05
comments: true
categories: [coding, edtech, pedagogy, education]
---

Recently, I bemoaned the [ill-preparedness of educators to teach programming](http://decomplecting.org/blog/2013/06/02/were-not-ready-to-teach-kids-to-code/). Nevertheless, many people and organizations are making a concerted effort to teach these skills, often professional software developers who are either volunteering their time or forming non-profits to introduce the students with the least access to instruction in the basics of programming.

While this is admirable, I think the most common current approach is compleely wrong-headed. One local non-profit I really admire and have high hopes for is [Code in the Schools](http://codeintheschools.org/). I was excited to hear that they recently secured 501(c)(3) non-profit status, and subsequently secured a grant from [The Awesome Foundation](http://www.awesomefoundation.org/) to run their 8-week programming course at Digital Harbor High School and Liberty Heights Elementary here in Baltimore. 

This is fantastic, in and of itself. But programs like this are (in the media, at least) [held up as examples](http://technical.ly/baltimore/2013/06/06/code-in-the-schools-gaming-legrand/) of addressing the issue that [Code.org](http://code.org) and [She++](http://sheplusplus.com) are addressing, notably the shortage of software engineers relative to the prospective demand for engineering job candidates in the future. And we are still failing.

<!-- more -->

This isn't a criticism of Code in the Schools. Teaching game programming is a really cool idea. And it sounds like fun; that's what I wanted to code in elementary school, and I had fun doing it on my Apple //e and my IBM PS/2. But it has nothing to do with the skills we're really demanding of today's kids, not only the prospective engineers, but ultimately every student we want to be successful in the world to come.

### Basic (Computational) Literacy

I could write a basically coherent 5-paragraph form essay by first or second grade. If I'd just continued to increase my vocabulary, I could have learned nothing else about language, and gotten high marks on the state assessment tests in 5th grade. If "teaching to the test" were enough, well, that would have been fine. But instead, I learned not only parts of speech, not only Greek and Latin roots, etymology, etc., not only what words meant, but _how_ words meant, and how to think critically about those meanings. In hindsight, I consider this a fundamental component of literacy.

Teaching kids to make video games with simple languages is like giving them Mad Libs: it demonstrates that language can be fun, and that it's more fun when you understand the basic concepts, but in no way is it necessary or sufficient for the conditions of "basic literacy."

In my last post on this topic, I introduced a concept I was calling "computational literacy," and cited [a similar EdSurge piece](https://www.edsurge.com/n/2013-05-28-opinion-learning-to-code-isn-t-enough) by [Shuchi Grover](https://www.edsurge.com/shuchi-grover).

My fear with these "let's make a game" approaches to programming is that while they teach the basics of creating a program that will compile and run (a feel-good achievement, but a very, very low bar, to be sure), they don't necessarily teach anything about computation. I'll come back to this, but for the moment I want to step into the Wayback Machine, all the way back to the prehistoric era of 2005.

### "The Perils of JavaSchools"

Back in '05, Joel Spolsky wrote a [somewhat controversial blog post](http://www.joelonsoftware.com/articles/ThePerilsofJavaSchools.html) of this title, lamenting the transition of Computer Science program curricula from (typically) C and Scheme to Java. (I don't think he knew how bad it was; as early as 1999 I skipped out on taking CS 101 because it was all Visual Basic, and I'd been running Linux for five years. Not. Even. Once.)

The takeaway from that article is that programs were selecting Java because fundamental CS concepts that were necessary to coding in C and/or Scheme (pointers and recursion... y'know, the Hard Stuff) could be glossed over in Java (automatic memory management, no TCO, just for() loops with no `malloc`s).

The dark side of this trend was that not only did it increase retention rates in CS programs by making the requirements easier, it also churned out a generation of sub-par engineers, fueling the (failed) movement to commodify software engineering.

As an aside, this is something else that concerns me from a historical-materialist standpoint: are we repeating the past?

It's worth noting that although the goals of Code.org and She++ are both noble and (perhaps) altruistic, their backers have a massive economic stake in this area. She++, for example, is sponsored by [Sequoia Capital](http://www.sequoiacap.com/), [Andreesen Horowitz](http://www.a16z.com/), [Oracle](http://oracle.com), [Intel](http://intel.com), [Microsoft](http://microsoft.com), and [Facebook](http://facebook.com), among others. Code.org's advisory board includes representatives from [Amazon](http://amazon.com), Microsoft, [Twitter](http://twitter.com), [Google](http://google.com), etc.

These are companies facing a real crisis that strikes at the core of their business as qualified engineers become increasingly scarce. They are also companies that are competing for top talent with starting salaries in the high $200k range. So mightn't they benefit from a re-commodification of software engineering?

I personally don't think it's realistic that we will see a renewed attempt to commodify engineering, at least not among top companies; they know what happened the last time, and a bad engineer can do more damage than an empty desk.

### Resources for Moving Forward

I want to look at some resources for teaching the kind of basic computer science we need students to learn. Most of these would be more appropriate for older students, but I'm confident that many of the concepts can be reframed in a context appropriate for students down to the primary school level.

##### Concrete Mathematics

{% img [float-right] http://ecx.images-amazon.com/images/I/518GBVWEBYL.jpg Concrete Mathematics %}

Just as computer science itself does, I'll start with mathematics. [Concrete Mathematics] is a textbook written by Ronald Graham, Donald Knuth (author of _[The Art Of Computer Programming](http://en.wikipedia.org/wiki/The_Art_of_Computer_Programming)_), and Oren Patashnik, who were dissatisfied with the resources available for teaching the mathematical foundations of computer science at the time.

Written in a humorous style, the book also slyly teaches fundamental concepts without explicitly stating intent. For instance, the first chapter explores the [Tower of Hanoi](http://en.wikipedia.org/wiki/Tower_of_Hanoi) game, teaching both recursion and computational complexity in the process.

The text is available as a [PDF download](http://www.cse.iitb.ac.in/~vsevani/Concrete%20Mathematics%20-%20R.%20Graham,%20D.%20Knuth,%20O.%20Patashnik.pdf)

##### Structure and Interpretation of Computer Programs (SICP)

{% img [float-right] http://upload.wikimedia.org/wikipedia/en/9/9d/SICP_cover.jpg SICP %}

SICP, also known as the Wizard Book, is perhaps the most famous CS text of all time, and with good reason. Originally developed by for MIT's introductory programming course 6.001, the book teaches the [Scheme](http://en.wikipedia.org/wiki/Scheme_(programming_language)) dialect of Lisp in the very first chapter, and goes on to build upon basic principles, up to and including writing a Scheme interpreter - in Scheme.

The text is available under a [Creative Commons](http://creativecommons.org/licenses/by-sa/3.0/) license from [MIT Press](http://mitpress.mit.edu/sicp/).

##### Understanding Computation

{% img [float-right] http://akamaicovers.oreilly.com/images/0636920025481/cat.gif Understanding Computation %}

A newer example from [O'Reilly](http://oreilly.com), [Understanding Computation](http://shop.oreilly.com/product/0636920025481.do) explores many of the core concepts of SICP, but in a more accessible style, and uses the [Ruby](http://ruby-lang.org) programming language for its examples. The first chapter, for example, iteratively builds up a virtual machine for a hypothetical programming language called SIMPLE. 

The book goes on to discuss automata theory, state machines, type systems, etc., eventually delving into Turing machines and the lambda calculus, finally exploring unsolvable problems in computer science, such as the halting problem.

The beauty of this text is that it explores major concepts in theoretical computer science in a way that is both accessible and enjoyable. Unlike the previous two suggestions, this is _not_ a textbook, but rather an invitation to further exploration, making it suitable for perhaps a younger audience than _Concrete Mathematics_ or _SICP._

##### Learn to Program

{% img [float-right] http://imagery.pragprog.com/products/139/ltp2_xlargecover.jpg?1298589829 Learn to Program %}

Targeted toward younger children, [Learn to Program](http://pragprog.com/book/ltp2/learn-to-program) teaches Ruby in a simple but coherent style, starting with one-line programs, and moving on to larger examples. Unlike other resources geared toward a younger audience, it not only provides answers to the problems posed, but it includes them both in a "how you _could_ do it" _and_ in a "best practices" style, so that learners are given the obvious answer and the right answer - and the difference is explained. 

### Doing It Right

The list above is by no means exhaustive, and certainly isn't suitable for all audiences. But I can't accept that building video games with [Kodu](http://www.kodugamelab.com/) or [SmallBasic](http://smallbasic.com/) is really addressing the fundamental problem of computational literacy.








