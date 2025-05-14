+++
title = "Post 1"
description = ""
date = 2022-01-01
updated = 2025-01-01
draft = false

[taxonomies]
categories = ["two"]
tags = ["one", "two", "three"]

[extra]
lang = "en"
toc = true
comment = false
copy = true
outdate_alert = true
outdate_alert_days = 120
math = false
mermaid = false
featured = false
reaction = false
+++

Rust 1.0 is on its way! We have nailed down a concrete list of features and are hard at work on implementing them. We plan to ship the 1.0 beta around the end of the year. If all goes well, this will go on to become the 1.0 release after the beta period. After 1.0 is released, future 1.x releases will be backwards compatible, meaning that existing code will continue to compile unmodified (modulo compiler bugs, of course).

Of course, a Rust 1.0 release means something more than "your code will continue to compile". Basically, it means that we think the design of Rust finally feels right. More specifically, it feels minimal. The language itself is now focused on a simple core concept, which we call ownership and borrowing (more on this later). Leveraging ownership and borrowing, we have been able to build up everything else that we have needed in libraries. This is very exciting, because any library we can write, you can write too. This really gives us confidence that Rust will not only achieve its original goals but also go beyond and be used for all kinds of things that we haven't even envisioned.

## The road to Rust 1.0
Rust has gone through a long evolution. If you haven't looked at Rust in a while, you may be surprised at what you see: over the last year, we've been radically simplifying the design. As a prominent example, Rust once featured several pointer types, indicated by various sigils: these are gone, and only the reference types (&T, &mut T) remain. We have also been able to consolidate and simplify a number of other language features, such as closures, that once sported a wide variety of options. (Some of these changes are still in progress.)
