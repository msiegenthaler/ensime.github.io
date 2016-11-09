---
layout: section
order: 99
title: Contributing
---

Contributions to the code and documentation are welcome!

## Improving The Documentation

Fork the [ENSIME site][ensime-site] on Github.


## Running from Source (C9 SDK)

To run the ENSIME plugin with a locally installed cloud9 environment

- install the Cloud9 SDK by following their [guide](https://cloud9-sdk.readme.io/docs/running-the-sdk)
- check out our git repository [ensime-cloud9](https://github.com/ensime/ensime-cloud9) into your `~/.c9/plugins` folder
- rename it to `c9.ide.language.scala` (or replace the already existing folder with it)
- do a `npm i ensime-controller-js` in your `~/.c9/plugins` folder
- Start using `./server.js -p 8080 -l 0.0.0.0 -a : -w ~/source/scala-example/` from the c9sdk folder (where ~/source/scala-example is your workspace root)
- inside your workspace add a symlink to your plugin `ln -s ~/.c9/plugins/c9.ide.language.scala ensime-plugin`
- open it in your browser to start developing
    - to develop: http://localhost:8080/ide.html
    - to test it: http://localhost:8080/ide.html?debug=2

Then fork the project on github and add pull requests to add features or to fix bugs.