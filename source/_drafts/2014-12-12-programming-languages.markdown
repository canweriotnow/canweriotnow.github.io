---
layout: post
title: "Programming Languages and Human Languages, with An Application to The Entscheidungsproblem"
date: 2014-12-11 21:59:34 -0500
comments: true
categories: [programming languages, language, philosophy, poststructuralism, entscheidungsproblem]
---

## Language

Language, particularly in this context, is a term which philosophers of language would suggest suffers from "symbolic overdetermination".

Ever since the beginning of higher-level languages (FORTRAN and LISP were the first, but DataFlow was in the works at the time), there has been a desire to create programming languages that mirrored human languages. DataFlow (managed by the inimitable Rear Admiral Dr. Grace Murray Hopper) eventually became COBOL, which for the longest time was the closest human/computer language synthesis that was actually executable/compilable.

It's gotten better, but not really.

<!-- more -->

## _Différance_

_Différance_ is a term first invented by Derrida in 1963, but more commonly associated with the essay "Différance" in _Margins of Philosophy,_ published in 1983.

The concept of _différance_ expresses a "middle voice" between the normal meanings of the French infinitive verb _differer_, which means both "to differ" and "to defer"

What Derrida desired to express with this term was that meaning in language was always _deferred_ until the next expression, and the next, _ad infinitum,_ and that because of this deferral the final meaning was inevitably _different_ to the speaker's original intent.

## And Programming?

It could never really function this way, could it? Eventually, we have to compile and at that point some things have to be fixed. Certainly, in Lisp we can defer evaluation until macroexpansion-time or compile-time, and we can modify code at runtime, but we still need some kind of final evaluation of forms at one point or another.

And this is where the metaphor of calling programming languages "languages" breaks down.

## The Halting Problem

This is Alan Turing:

{% img center /images/post-img/turing1.jpg %}

You probably know of him from his work on decrypting the Enigma cipher at Bletchley Park during World War II, but before that he wrote one of the most important texts in the corpus of computer science history: In May of 1936, he wrote ["On Computable Numbers, with An Application to The Entscheidungsproblem"](http://www.cs.virginia.edu/~robins/Turing_Paper_1936.pdf) [PDF].

In this paper, he devised the notion of the "Turing Machine", a universal computer that could calculate any computable function give an infinite loop of paper tape on which to read or write symbols.

(As an aside, Alonzo Church was working on a similar problem down the hall at Princeton, and demonstrated equivalent results with his lambda calculus; this is why we describe our model of computation as the Church-Turing Thesis)

Back to the problem at hand: the _Entscheidungsproblem_ was a problem described in the 19th century by the mathematician David Hilbert; it roughly translates to "decision problem." Turing took a particular case of the _Entscheidungsproblem,_ the halting problem, and used it to prove the point.

The interested reader may explore how Kurt Gödel's Incompleteness Theorem factors in, but such an explication is beyond the scope of this essay.

Anyhow, Turing's work in this case was to demonstrate that given a function, and a set of inputs, it was **not** possible, in advance, to know whether the operation would terminate and/or return a value.

If Derrida is correct, and the meaning of natural language is always differing/deferred, than any operation performed on it is necessarily non-halting. Since the parser for natural languages is the human brain and _not_ a Turing Machine, language _works,_ but the fact that it does is an interesting problem in itself.

I won't do a deep-dive into the chain of reasoning from de Saussure to Derrida and beyond, but the post-structuralist notion that language works precisely due to its "brokenness" is one I've been exploring since high school.

Returning to the question of the impedance mismatch between mind and machine, I'd like to explore some potential points of impact.

### Natural Language Processing

### Strong AI
