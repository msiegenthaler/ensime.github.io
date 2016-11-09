---
layout: section
order: 1
title: Installation
---

## Installation on c9.io

Before you start make sure you have a working c9.io account and an open workspace with
a Scala project using SBT. The project should have a `build.sbt` in the workspace root.
The type of the project does not matter, choose _blank_.

*Cloud9 seems to have some trouble with their package manager at the moment, so we're unable
to support it at the moment.*

If you still want to try it then you can basically follow the "Install plugin from source" step
from the local installation and then add a `?debug=2` to your c9.io workspace URL (Example: `https://ide.c9.io/msiegenthaler/my-project?debug=2`).




## Local Installation

- Install the cloud9 SDK (for details refer to their [installation page](https://cloud9-sdk.readme.io/docs/running-the-sdk)).
      `
      git clone https://github.com/c9/core.git c9sdk
      cd c9sdk
      ./scripts/install-sdk.sh
      `

- Install the plugin from source
      `
      mkdir -p ~/.c9/plugins
      git clone -b v1.1 https://github.com:ensime/ensime-cloud9.git ~/.c9/plugins/c9.ide.language.scala
      `

- Start the IDE (in the example we're using ~/source/scala-example as our project)
      `
      ./server.js -p 8888 -l 0.0.0.0 -a : -w ~/source/scala-example/
      `

- Open the IDE in the webbrowser: `http://localhost:8888/ide.html`

