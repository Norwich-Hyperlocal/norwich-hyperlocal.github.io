---
layout: post
title: "Install Python and PIP with homebrew on OSX"
date: 2014-07-30 12:10:25
categories: Homebrew Tutorial PIP
---

So I did not have PIP installed but I had Python installed, so to fix this I reinstalled python to make sure.

So we want to install PIP as its a tool for installing and managing Python packages. [see more here](https://pypi.python.org/pypi/pip)

Firstly we need to have homebrew installed [do this here]({% post_url 2014-07-30-install-homebrew-on-osx %})

Then we run

    brew install python

And get lots of this in the console output:

![Console output](/images/screenshots/homebrew-python.png)

Finally when that has finished we write,

    python -V

Note big V, and the following:

    pip -V

We get something like the following output, which shows that python and pip are not available.

![versions](/images/screenshots/homebrew-python-pip.png)