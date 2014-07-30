---
layout: post
title: "Install Flask for python"
date: 2014-07-30 12:10:25
categories: Homebrew Tutorial Flask
---

As long as you have [pip and python installed]({% post_url 2014-07-30-install-pip-using-homebrew-on-osx %})

We'll use virtualenv to install Flask. Virtualenv is a useful tool that creates isolated Python development environments. So run the following:

    sudo pip install virtualenv

Note we run this using "sudo" as an admin so its installed for all users on the computer. You get the following output:

![Console output](/images/screenshots/virtual-env-console.png)

So now when we run:

    virtualenv --version

We get:

![Console output](/images/screenshots/virtualenv-version.png)

So that was successful as we not have a version number showing. I already had a folder setup with a repository so I ran the following outside the folder:

![Console output](/images/screenshots/virtual-env-setup.png)

if I go into that directory and list the contents using:

    ls -al

I get the following:

![folder listing](/images/screenshots/virtual-env-folder.png)

So things looking good. Now if we run the following to active the virtual environment and then we can work without affecting the computer libraries:

    . bin/activate

You should see (APPNAME) at the begining of the console line:

![console activate](/images/screenshots/virtual-env-activate.png)

Now we run:

    pip install Flask

To check if everything is good we can now can goto the python console in the command line, Do this by just typing in python:

![python console](/images/screenshots/python-console.png)

So now type in the following, pressing return inbetween to run the command:

    import flask
    flask.__version__

And you can now see the version number:

![Flash version](/images/screenshots/flask-version.png)

Now you can install Flask for your projects.

