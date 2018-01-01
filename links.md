+++
author = "Alex Addy"
title = "Useful Links"
+++

This page is a collection of pages and projects that I personally find
interesting or useful.

# General Programming Links

## Time

 - [The Problem with Time & Timezones](https://youtu.be/-5wpm-gesOY) is an
   excellent short video explanation of just how hard it is to deal with
   timezones. There is a very relevant [xkcd](https://xkcd.com/1883/).

 - [Roughtime](https://int08h.com/post/to-catch-a-lying-timeserver/) is an
   attempt at dealing with some of the problems concerning ntp. By only
   requiring accuracy within a few seconds of real time Roughtime is able
   to make a scalable and secure time protocol.

 - [Keeping Time in Real Systems by Kayva Joshi](https://youtu.be/BRvj8PykSc4): 
   this video covers the problems of time when the goal is high precision
   and accuracy. Then goes further to cover the much more difficult task of
   timekeeping in a distributed system.

# The Rust Programming Language

 - [Fireflowers](https://brson.github.io/fireflowers/): a great collection of
   commentary explaining why people use Rust and what it is trying to do.

 - [The Rust Book 2E](https://doc.rust-lang.org/book/second-edition/) is the
   core book for learning Rust. It is written for those with some programming
   experience and does not cover basic programming concepts. It will soon be
   published physically and can be pre-ordered [here](https://www.nostarch.com/Rust).

 - [Rust by Example](https://rustbyexample.com/) is a collection of many self
   contained examples useful for many locations in a rust program. It is best
   used as a supplement to the Rust Book.

 - [The Rust Standard Library](https://doc.rust-lang.org/std/): this reference
   is very complete and well done. I always end up with several tabs open to
   this when programming.

 - [Rust Cookbook](https://rust-lang-nursery.github.io/rust-cookbook/) is
   a collection of high-quality crates arranged by task and topic. Very useful
   when trying to determine what crate to use for a task.

 - [Learning Rust link collection](https://github.com/ctjhoa/rust-learning):
   go here for an even larger collection of resources for learning Rust.
   The links are useful for all levels of Rust users.

## Rust Design

 - [Rust API Guidelines](https://rust-lang-nursery.github.io/api-guidelines/)
   a very useful book if you are looking to make a crate of your own. Reading
   and understanding the guidelines in this book will help your crate have
   a higher quality from the start.

## Projects

 - "[Tock](https://www.tockos.org/) is an embedded os for running multiple
   concurrent, mutually distrustful applications on Cortex-M embedded
   platforms."

 - [Gotham](https://gotham.rs/) is an async web framework for rust that looks
   to be a fairly easy way to get a webserver made in with minimal fuss.

 - [Rocket](https://rocket.rs/) is another web framework that eliminates
   boilerplate and provides type-safe web programming. The only downside being
   that it currently depends on a bunch of experimental language features. A video
   explaining how Rocket works can be found [here](https://youtu.be/t_FUZ34ahBE).

 - [RustAudio](https://github.com/RustAudio/) is a collection of free and useful
   audio, DSP, and music libraries.

 - [Rayon](https://github.com/rayon-rs/rayon) is a library with the goal of
   making it easy to add parallelism to sequential code. It's way of providing
   easy, data-race free, parallelism makes it an excellent tool in the toolbox.

 - [Specs](https://slide-rs.github.io/specs-website/) is a high-performance
   Entity-Component-System library written to provide flexibility and easy
   parallelism. It is mainly intended for use in games where the ECS design
   pattern is used to great effect.

 - [Failure](https://github.com/withoutboats/failure) is a crate that can
   be used to manage your error types. It is the successor to
   [error-chain](https://github.com/rust-lang-nursery/error-chain), and is
   the next step on managing complex projects with many Error types. The
   introductory blog post [here](https://boats.gitlab.io/blog/post/2017-11-16-announcing-failure/)
   explains why Failure was deemed necessary.

## Blog Posts

 - [Portability Concerns with Path](https://udoprog.github.io/rust/2017-11-05/portability-concerns-with-path.html):
   a blog post concerning the difficulty of dealing with the same path
   in a cross-platform environment, such as in a project manifest that
   has to work on windows and linux. Introduces a new crate to assist with
   this use case.

 - [Securing the Foundations of the Rust Programming Language](https://www.ralfj.de/blog/2017/07/08/rustbelt.html)
   concerns formal proofs of Rust's ownership and type system in several of its
   core libraries.

 - [Rust Performance Pitfalls](https://llogiq.github.io/2017/06/01/perf-pitfalls.html)
   discusses a number of performance pitfalls in Rust and provides examples of how
   to resolve them.

 - There is a great effort in the community to improve the ergonomics of Rust. As
   part of this effort Aaron Turon made an excellent [post](https://blog.rust-lang.org/2017/03/02/lang-ergonomics.html)
   outlining what exactly is meant by "ergonomics" through an approach expanding
   on the idea of a "reasoning footprint". A related post [here](https://boats.gitlab.io/blog/post/2017-12-27-things-explicit-is-not/)
   covers what explicit is and isn't in order to encourage the use of more precise
   terms such as "noisy", "local", "manual", etc.

 - [Rust lifetimes: Getting away with things that would be reckless in C++](http://www.randomhacks.net/2014/09/19/rust-lifetimes-reckless-cxx/):
   illustrates what can be gained through the additional safety guarantees that
   Rust provides.

 - [Mentally Modelling Modules](https://manishearth.github.io/blog/2017/05/14/mentally-modelling-modules/):
   this the best resource to understand the current module system. Anyone stuck
   trying to figure out how Rust modules to work needs to read this post.

 - [Undefined vs Unsafe in Rust](https://manishearth.github.io/blog/2017/12/24/undefined-vs-unsafe-in-rust/)
   is a short post that clearly lays out what the words "unsafe" and "undefined"
   mean in Rust. It was made in response to this [post](https://jvns.ca/blog/2017/12/23/segfault-debugging/)
   dissecting a segfault that is the result of undefined behavior stemming from
   calling unsafe functions incorrectly; it's a fun post, go read it.

# The C++ Programming Language

 - [Understanding Strict Aliasing](http://cellperformance.beyond3d.com/articles/2006/06/understanding-strict-aliasing.html)
   thoroughly explores what strict aliasing is and its impact on the correctness
   and speed of a variety of C++ snippets. This is an advanced topic but C++ and
   C programmers should be aware of its impact on what pointer behavior is and
   isn't defined in order to avoid difficult to track down bugs.

