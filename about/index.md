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

## How to run experiments

Find an experiment, either by looking at the
[list of all experiments](index.html), or searching by category in the menu on
the left. Click **Start Experiment** to launch the desired
experiment. Experiments should run smoothly in any up-to-date web browser, but
if you are having trouble try running the experiment in
[Google Chrome](http://www.google.com/chrome).

## How to modify experiments

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

#### Step 2: Fork the FactorsDB repository.

Go to the [GitHub page for FactorsDB](http://github.com/jodeleeuw/factorsdb) and
click the Fork button near the top right corner of the page.

**IMAGE HERE**

#### Step 3: Find the experiment you want to modify.

All of the experiments on FactorsDB are contained in the `_experiments/` folder
of the repository. Open the folder to view a list of all the experiments. Find
the one you want to modify and click on the filename to open it in the GitHub
viewer. Then click the edit icon (pencil) near the top right corner of the
document.

**IMAGE HERE**

#### Step 4: Edit the document and commit your changes.

Edit the experiment file as you see fit. Create a new commit by writing a brief
commit message in the box below the file contents and then click the green
**Commit Changes** button. Make sure to select the option *Commit directly to
the gh-pages branch*.

Experiments on FactorsDB are written in JavaScript using the
[jspsych library](http://www.jspsych.org). You can learn more about how jspsych
works by reading the [jspsych documentation](http://docs.jspsych.org).

#### Step 5: View your modified experiment.

Once you have forked and made at least one change to the repository, GitHub will
automatically build a new copy of the website linked to your account. You can
view your copy of FactorsDB by going to
http://<your-user-name>.github.io/factorsdb. For example, my GitHub user name is
*jodeleeuw*, so I would go to [http://jodeleeuw.github.io/factorsdb].

## How to contribute an experiment

Contributing an experiment is a similar process to modifying an experiment, with
a few extra steps. Follow the steps described above to create a GitHub account
and fork the FactorsDB repository. Then follow the steps below.

#### Step 1: Add a new .html file to the _experiments folder

All experiments are stored in the _experiments folder in the repository. To add
a new experiment, create a new .html file in that folder. You can either create
an empty .html file, or copy and rename one of the existing .html files. The
copy-and-rename strategy has the added benefit of giving you a template to
modify.

#### Step 2: Create the front matter

At the top of all experiment files is a section called *front matter*. This is a
term from the [Jekyll engine](http://jekyllrb.com/docs/frontmatter/) used to
render the GitHub repository into the FactorsDB website. The front matter is
written in [YAML](http://yaml.org/). This section is where
various experiment parameters are specified. The valid parameters are:

* `title`: The title of your experiment.
* `description`: A description of your experiment.
* `jspsych_version`: The version of jspsych used to run your experiment.
* `required_plugins`: The jspsych plugins that are required to run the
experiment.
* `categories`: The experiment categories that your experiment belongs in.

#### Step 3: Write the experiment code

The rest of the file contains the JavaScript code to run your experiment. You do
not need to write any of the standard HTML; it will be automatically rendered by
Jekyll. The output HTML body tag contains a div with the ID jspsych-target:
```html
<body>
  <div id="jspsych-target"></div>
</body>
```
You should use `$('#jspsych-target')` as the parameter for `display_element` in
the `jsPsych.init()` call for your experiment.

#### Step 4: Submit a pull request on the FactorsDB repository

Once you are done writing your experiment, you can submit a pull request to
merge your changes with the FactorsDB repository. For more information about how
to submit a pull request, see the GitHub documentation on
[using pull requests](https://help.github.com/articles/using-pull-requests/).
