---
layout: section
order: 1
title: Cloud9
---

Cloud9 is an online IDE with may supported language - thanks to ENSIME also with scala.
It runs our own private workspaces inside Docker containers and even lets you install
custom software.

![ENSIME Cloud9 screengrab](img/screenshot.png)

There's also an Open Source variant available that you can run on your own server (SDK). See
Usage of the SDK is restricted to non-commercial, see the [licensing documentation](https://cloud9-sdk.readme.io/docs/the-licenses-for-cloud9-sdk-and-packages).

Supported features include:
- code completing
- error highlighting
- show type of expression (in tooltip)
- show documentation (in tooltip)
- format code
- organize imports


## Motivation
As compiling Scala code is very CPU intensive - even more so you auto-run the
tests (i.e. using `sbt ~test-quick`) - the laptops we work on are too slow
and the battery runs down very fast.

But most of us have powerful servers available - why not let them do the heavy
lifting and just do the code browsing and editing on your local machine?


## Getting Started

see our [installation guide][installation]



## Get Involved
See our github project [ensime-cloud9](https://github.com/ensime/ensime-cloud9).

How to help:
- Raise issues for things that do not work
- install the current development version - see [development]


[installation]: installation
[development]: development
