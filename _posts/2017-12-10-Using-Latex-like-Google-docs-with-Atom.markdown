---
layout: post
title: Collaborate on Atom for Scientific Writing using Latex; Like using Google docs
date:   2017-12-08 17:11:36 -0800
comments: true
categories: jekyll update
---

In this post, I will show you how to use to packages in the atom text editor, to collaborate on scientific papers using latex just like you would do on google docs.

## Steps:

- Download and install [atom](https://atom.io/).

### Latex Setup

- From the top menu select packages, then Settings View and then Open.
- Select + Install tab on the left sidebar.
- Search for latex.
- Install the latex package by thomasjo.
- Then test it if it works.
- Use the first example I found on google [here](http://www.cs.technion.ac.il/~yogi/Courses/CS-Scientific-Writing/examples/simple/simple.htm).
- Copy paste the tex file shown on this website on your machine and open it using atom.
- Requirements for this Latex package is to have Latex installed on your machine. Install latex from [here](https://www.latex-project.org/get/).
- Hit Packages again on your top menu again and select Latex and build.
- Your latex file must render and you will be able to view it.

### Collaboration setup

- From the top menu select packages, then Settings View and then Open.
- Select + Install tab on the left sidebar.
- Search for atom-pair.
- Install the atom-pair package by pusher.
- Go back to your tex file in atom.
- Hit Packages again from the top menu bar and select Atom Pair. Then Select Start New Pairing Session.
- Your session ID will be automatically copied in your clipboard.
- Share this ID with your collaborators.
-

- Requirements for the collaborators:
  - Have atom-pair installed if they just want write in your latex document.
  - Have Latex for atom installed if they want to also render the latex file into a pdf.
