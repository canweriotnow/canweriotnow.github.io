---
layout: post
title: "Reflections on Rails (from Clojure)"
date: 2014-11-23 20:50:58 -0500
comments: true
categories: [clojure, ruby, rails, coding]
---

I've noticed this trend online, but it was even more pronounced at [Clojure/conj](http://clojure-conj.org)... a _lot_ of Clojure hackers are coming from [Ruby](http://ruby-lang.org). And most of us did a lot of work with [Rails](http://rubyonrails.org).

I'm not hating on Rails. But the more work I do in Clojure (especially where web dev is concerned), the more pronounced the philosophical differences become. I still maintain one (maybe one and a half, it's a bit muddled) Rails applications, so I still have one foot in that world, but it's increasingly like having one foot in... something not very pleasant.

Rails served me very well for many years. Ruby was a revelation, coming from Perl, and having a sophisticated framework to bootstrap a web project was like magic. When I made the decision to migrate a legacy Perl CGI codebase to Rails, my co-worker was dubious due to Rails' level of "magic."

That project is the subject of my "Legacy Systems on Rails" series (which [starts here](http://decomplecting.org/blog/2012/08/02/legacy-systems-on-rails-part-1/)), and it was a successful project, and I'm not sure that (at the time) I could have pulled it off differently. But times change.

## Frameworks

Object-oriented programmers seem to love their frameworks. Rubyists have Rails and [Padrino](http://www.padrinorb.com/), Java programmers have [Struts](http://struts.apache.org/) and [Spring](http://spring.io/), Pythonistas have [Django](https://www.djangoproject.com/), and... well, let's not pretend I'm going to condescend to address PHP, or consider it OO, but there are frameworks.

Functional programmers tend to eschew frameworks in lieu of simple, composable components. The closest thing we have to a "framework" in Clojure-land is [Luminus](http://www.luminusweb.net/), and it's more of a template (actually, it's primarily a [Leiningen](http://leiningen.org/) template for web applications) with a host of options for fine-tuned choices of which components to include or exclude.

There's nothing inherently wrong with frameworks; they tend to bump you up a level of abstraction and, in the case of opinionated frameworks like Rails, save you a bunch of configuration time. But that's not always what you want.

## Complexity

One of the things I loved about Rails, especially when I was building a system that interfaced with a vendor database with over 500 tables and hundreds of stored procedures and package functions. I had to do some crazy voodoo (series cited, but there was even more) to deal with datetimes, composite primary keys, views with a dozen self-joins due to incompatibility between insane vendor DBAs and insane client demands, but... Ruby and Rails did make my life easier even if I was monkey-patching `Float` for dubious reasons.

The thing that eventually bit me in the ass was the masking of complexity.

In his essay ["No Silver Bullet"](http://en.wikipedia.org/wiki/No_Silver_Bullet), Fred Brooks distinguishes between essential complexity and accidental complexity. These are also known as "intrinsic" and "incidental" complexity. I prefer the latter terms, so I will adopt those.

Rails (and other frameworks) tend to be popular for the very reason that they obfuscate intrinsic complexity. But this is (almost?) always at the cost of incurring incidental complexity.

ActiveRecord is the best example of this, I think; it obscures the intrinsic complexity of SQL (and relational algebra itself, through ARel). For most cases, it does generate efficient SQL, especially when the tables in question have been generated with vanilla ActiveRecord migrations. In other cases... not so much. There are a plethora of gems out there that alter or monkey-patch ActiveRecord for alternate cases, [composite_primary_keys](https://github.com/composite-primary-keys/composite_primary_keys) (Side note: I think my first accepted PR on Github was to CPK). And with Ruby, you can always monkey-patch AR yourself... and then you should be questioning some of your previous decisions.

## Composing

One of the pain points I had with ActiveRecord was with queries that weren't directly table-related. Since tha pattern was to match classes to tables, the options were to create a view and override all the write methods to prevent uncaught exceptions, or to use weird join methods that didn't return what you'd expect.

So, composition: let's start with the database layer. Using [Korma](http://sqlkorma.com) or even straight JDBC, I get a basic data structure I can traverse in any of the normal ways, rather than an instance of `Person` for which I have to remember all of the class-specific methods, etc. I can do regular hashmap fns or use clojure.walk fns or whatever I want.

At a higher level, (web-stack-wise), I find the functional style easier to reason about. Routing in [Compojure](https://github.com/weavejester/compojure) is similar in many ways to [Sinatra](http://www.sinatrarb.com), except it uses the `defoutes` macro to define routes in an easily composable fashion.
