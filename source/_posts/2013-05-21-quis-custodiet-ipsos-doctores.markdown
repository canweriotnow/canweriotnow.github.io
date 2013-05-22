---
layout: post
title: "Quis Custodiet Ipsos Doctores?"
date: 2013-05-21 21:22
comments: true
categories: [coding, edtech, pedagogy, education]
---

I'm really excited about the heavy emphasis I'm seeing on [teaching kids to code](http://gettingsmart.com/2013/05/teaching-kids-to-code-an-economic-social-justice-issue/). Although I agree with just about everything [Jeff Atwood](http://codinghorror.com) wrote in his controversial post, ["Please Don't Learn to Code"](http://www.codinghorror.com/blog/2012/05/please-dont-learn-to-code.html) (read it if you haven't), I also believe that in an age in which [software is eating the world](http://online.wsj.com/article/SB10001424053111903480904576512250915629460.html), understanding code is a basic literacy issue. This goes beyond the concept of digital literacy: as applied, this boils down to knowing how to use Google. What we're seeing in the movement to bring coding into the core curriculum is a new emphasis on what I'd like to call _computaional literacy._ 

## Computational Literacy

Computational literacy is a concept that I wish had been "a thing" when I was in school. I'll start with an anecdote, and then delve into the gritty challenges that the "teaching kids to code" movement is (IMHO) failing to recognize.

When I was in middle and high school, I loved math... when they didn't make me do rote calculation. I learned BASIC when I was 5 or 6, so when I discovered that the Texas Instruments graphing calculators we were required to buy for class spoke just about the same dialect of BASIC I had learned as a kid (I first learned to code on a TI 99/4A), I was so excited. Once I could derive the algorithm from a new concept we were being taught, I could express it in code and skip the boring parts. I've never done well when bored.

Alas, my youthful optimism was to be dashed on the rocks of pedagogical ifnorance and stupidity. First, I was told that I wouldn't receive correct answers because I didn't "show my work". 

On the next exam, I wrote out the source listing of each program I had used with a reference to the problems to which it had been applied (I'm pretty sure the number of GOTOs I used in those days would have mande Dijkstra cry). 

That's when they usually called my mom in for a conference.

<!-- more -->

## WTF Technophobes

I have to give my mom props here. She's not a huge nerd like me, but she was the EdTech liaison for the school where she taught, and was _way_ more technical than any of the teachers I had in the same school district (actually, she used to teach the in-service courses on basic computer skills for the entire district; I completed my student service learning hours assisting in those classes). 

We went into those meetings facing an irate math teacher discussing how I was being insolent and writing a program instead of learning the math concepts I was supposed to learn in the class. My mother's response was a deadpan "If he didn't understand the concepts, how could he write the program?"

Did I mention my mom is awesome? She was no stranger to ignorance and technophobia, btw. She created one of the first computerized grade reporting systems in the state, initially with a Microsoft Works database, later with Filemaker Pro, and later still with Access (yeah, it's not Postgres, but it was the 90's, in an elementary school).

There was never a real resolution to this. I stopped taking math when I'd gotten enough credits to graduate (thanks, all my math teachers, for teaching me to hate a subject I once loved because it was taught by ignorant technophobes). I tried again in college, but was greeted by the same attitude, so combined with that and required CS 101 class on Visual Basic (as if I would run Windows, or write VB), I majored in Philosophy. Okay, that's enough spleen for this post (and I have no regrets majoring in Philosophy; you'll learn more critical thinking skills in a good philosophy program than in any Applied Math or CS program).

## Teaching Kids to Code? Why?

We need a paradigm shift in education before we even _dream_ of making coding part of the curriculum. Until we challenge our basic attitudes and assumptions, teaching kids to code in school will be an abject failure, for a number of reasons.

The first is that abstract learning without application is meaningless. I'm not the most emotive viewer, but Conrad Wolfram did a TED talk a while back that had me jumping out of my chair, clapping, and shouting "#{expletives.sample} yeah!" repeatedly at my computer. Here's the video (If you haven't watched "Teaching kids real math with computers", do so NOW):

<iframe width="560" height="315" src="https://www.youtube.com/embed/60OVlfAUPJg" frameborder="0" allowfullscreen></iframe>

If our math curricula (the subject best suited to a programming solution!) are based around chidren doing rote, repetitive calculation, what's the point in teaching them to code? I had hoped that maybe "it gets better" applied to the attitude toward programming in schools, but a quick Google search showed that not much has changed, e.g. [Washington's state K-12 math calculator policy](http://www.k12.wa.us/mathematics/CalculatorPolicy.aspx).

No programs. No code, dogs, or Irish need apply.

How can we even _think_ of teaching kids to code while code is a "cheat," "not showing your work" (where's the harm in automating work that _should_ be considered beneath human dignity?), et cetera.

Most of the proposals I've seen around the "teaching kids to code" thing center on getting practicing software engineeers to volunteer their time with kids to teach them basic (and more advanced, if they're into it) programming skills.

We're totally into this idea! Particularly in the Ruby community, there's [KidsRuby](http://www.kidsruby.com/) and [Hackety Hack!](http://hackety.com/), awesome projects centered around teaching kids basic programming skills in a fun and easy-to-learn dynamic language.

But until teachers understand the tech enough to embrace (rather than fear) it, what's the point?

If I wasn't already at least a hobbyist hacker, and I was taking my first programming course, and arrived in math class only to be told I couldn't apply my exciting and newly-learned skills to the problem at hand, because it was like cheating, how would I react? I'd most likely lose interest in a subject I couldn't apply to anything.

Okay, well, _I_ would likely lose interest in my math class (or at least my math teacher) because code is _so frakking cool._ But I'm trying to imagine myself as the student who isn't a huge nerd.

## Quis custodiet ipsos custodes?

It might sound like I've been a bit harsh toward the teachers here. Nothing could be further from my intent. As I've gained time and distance, I've realized that it's merely ignorance that built a wall between us; not stupidity, and certainly not malice. And it was an ignorance for which they were not responsible; it was the fault of the system that trained them, and the system that was later responsible for their professional development.

No one ever taught my teachers about software; what went into building it, using it, etc.

If (most of) the teachers are computational illiterates, how can we expect the kids to become computationally literate in any meaningful way? 

Technology has penetrated pedagogy to a significant degree but hasn't really changed the practice in a fundamental way; if your use of technology isn't transformative, it's a misuse, possibly an abuse.

Where technology hasn't penetrated in a meaningful way is in professional development. Teachers are still "improving" their skills in more or less the same way they were decades ago. This has to change. If you're teaching in a STEM-related area and you don't (or won't) understand variable assignment, iteration, recursion, and other basic concepts &mdash; the very basics of coding &mdash; you should find a new career. I'm not saying you need to delve into pointers, concurrency, etc. Just the basics. If I were going into high school all over again (and this is what I intend for my daughter (if she's into it), so Math Teachers Beware!), I would go in with a mastery of [SICP](http://mitpress.mit.edu/sicp/), and a willingness to get myself expelled for refusing to do rote calculation when I could solve the problem with a 3-line recursive function in Scheme.

## What's The Answer?

Good question. I think the reason we don't have a good answer yet is that we've been asking the wrong question. Getting developers to mentor students is a fantastic idea; if my time wasn't 120% consumed between a startup and a six month old, I'd be spending my free time (that's a thing?) volunteering to teach kids to program. But we run into a roadblock when the general population of educators need a class just to use Twitter. Which is why I ask, "Quis docet ipsos doctores?" &mdash; "Who teaches the teachers themselves?"

This is also why I'm so excited about [An Estuary](http://anestuary.com). The opportunity to bring technological solutions not just to education, but to professional development within education, is the opportunity to bridge the gap between what students need to learn and what teachers are capable of allowing them to learn in a meaningful way. Of bringing education into the 21st century (after dragging it kicking and screaming through the 20th, because it's currently stuck in the 19th, albeit with some toys from the future).

I never want another child to look at her teacher and think (as I did) "are you from the past?" I never want another nerd to hate math because his teacher didn't understand the concept of an algorithm. I never want another hacker to give up on education because her teachers, professors, peers, etc. appeared to be stupid or malicious when they were merely ignorant. 

I want to change the system. I want to make "it gets better" real for hackers and nerds. 

I want to end the subjugation of billions of children to the subhuman task of rote calculation a thing of the past.

How far am I willing to go? 

Doctores docebo, si necesse est.

We must teach the teachers, or teaching the children is so much tilting at windmills. There are no easy solutions, but I'm proud to be part of a company addressing the hard solutions.

