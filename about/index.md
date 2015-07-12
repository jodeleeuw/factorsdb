---
title: FactorsDB - About
layout: default
---

# About

<p class="lead">FactorsDB is an open-source repository of experiments that
run natively in a web browser.</p>

FactorsDB was created to curate a collection of high-quality browser-based
experiments for classroom demonstrations. The experiments require no additional
software to run, making it easy for instructors and students to use the
experiments in a classroom setting. Anyone is free to use, contribute to, or
modify the experiments on this site. The site is hosted on GitHub and the entire
contents of the site is a
[GitHub repository](http://github.com/jodeleeuw/factorsdb).

All of the experiments on FactorsDB are created with the
[jspsych](http://www.jspsych.org) experiment library. jspsych is a free,
open-source JavaScript library for creating behavioral experiments that run in a
web browser.

FactorsDB was created by [Josh de Leeuw](http://pages.iu.edu/~jodeleeu) at
Indiana University.

## How to use FactorsDB for classroom demos

Find an experiment, either by looking at the
[list of all experiments](index.html), or searching by category in the left nav
on the [main page](index.html). Click **Start Experiment** to launch the desired
experiment. Experiments should run smoothly in any up-to-date web browser, but
if you are having trouble try running the experiment in
[Google Chrome](http://www.google.com/chrome).

## How to modify experiments on FactorsDB

The entire contents of the FactorsDB site exists as a
[GitHub repository](http://github.com/jodeleeuw/factorsdb). You can create a
copy of the repository and publish your own version of the site with just a few
clicks. Then you can modify any of the experiments on the site by editing the
experiment file. This is a great way to let students try variations of different
experiments for a project, or to learn how to use
[jspsych](http://www.jspsych.org).

#### Step 1: Create a GitHub account.

You will need a free GitHub account to fork (copy) the FactorsDB repository.
[Sign up here](http://www.github.com/join).

##### Step 2: Fork the FactorsDB repository.

Go to the [GitHub page for FactorsDB](http://github.com/jodeleeuw/factorsdb) and
click the Fork button near the top right corner of the page.

**IMAGE HERE**

###### Step 3: Find the experiment you want to modify.

All of the experiments on FactorsDB are contained in the `_experiments/` folder
of the repository. Open the folder to view a list of all the experiments. Find
the one you want to modify and click on the filename to open it in the GitHub
viewer. Then click the edit icon (pencil) near the top right corner of the
document.

**IMAGE HERE**

### Step 4: Edit the document and commit your changes.

Edit the experiment file as you see fit. Create a new commit by writing a brief
commit message in the box below the file contents and then click the green
**Commit Changes** button. Make sure to select the option *Commit directly to
the gh-pages branch*.

Experiments on FactorsDB are written in JavaScript using the
[jspsych library](http://www.jspsych.org). You can learn more about how jspsych
works by reading the [jspsych documentation](http://docs.jspsych.org).

### Step 5: View your modified experiment.

Once you have forked and made at least one change to the repository, GitHub will
automatically build a new copy of the website linked to your account. You can
view your copy of FactorsDB by going to
http://<your-user-name>.github.io/factorsdb. For example, my GitHub user name is
*jodeleeuw*, so I would go to [http://jodeleeuw.github.io/factorsdb].
