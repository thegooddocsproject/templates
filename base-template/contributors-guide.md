# Contributors' Guide

This guide covers how to get started with contributing to the Good Docs Project, including working with the project's code repository, and making your first pull request.
It does not cover how the project handles governance issues such as decision making and community roles and responsibilities.
For information about project governance, see [https://thegooddocsproject.dev/community.html](The Good Docs Project Community).

## Welcome to The Good Docs Project

## Welcome to The Good Docs Project

The Good Docs Project provides a set of templates and other resources to help you create great documentation.
Anyone can come and make use of those resources, download the templates, and create their own documentation at any time.
If you have a great idea for improving any of the resources, we would love for you to share them!
This guide is to help you get started contributing to the Good Docs Project, whether you intend to contribute a whole new template to the collection, or fix a typo.

## Getting Familiar with the project repositories

The source code for the Good Docs Project is in github, including the code for the website, example project, community governance, and the templates themselves.
Browse the code by navigating to [https://github.com/thegooddocsproject/] in your browser.

The Good Docs Project contains repositories for the templates,website, governance, and more.
To contribute to the templates, you need to work with the `templates` repo, and the `incubator` repo.

### The `templates` repository

This is the main repository in the project.
It contains the templates, and their companion guidance documents.
To make a small change to an existing template, such as updating some wording, or fixing a typo, propose a change directly within this repository.

### The `incubator` repository

For bigger projects, including creating a new template, use the `incubator` repository.
Use this repository to work on changes in collaboration with the rest of the community, and move it into the appropriate location when complete.

## Setting up your work environment

To work on content within the Good Docs Project, you need to set up your work environment.

### Selecting a text editor

A large range of text editors is available for download.
Your operating system will provide a simple text editor by default:

| Operating System | Editor   |
| ---------------- | -------- |
| Windows          | Notepad  |
| MacOS            | TextEdit |
| Linux - Gnome    | gedit    |
| Linux - KDE      | KWrite   |

Once you've gotten started with a basic editor, you'll have a better idea of what features you want in a more advanced editor.

### Working with git

You need to create a fork of the repository you want to contribute to.
A fork copies the current state of the repository to your own project.
When you have made your changes, you can propose the changes back to the original project with a pull request.
The community reviews your pull request, and you can make more updates or changes as needed.
When everyone agrees, the pull request gets merged, and your changes become part of the code.

This example uses the `incubator` repository, but the method is the same for any repository.
If you need more help with git, check out the github documentation at [https://docs.github.com/].
For a glossary of git terms, see [The git glossary](https://mirrors.edge.kernel.org/pub/software/scm/git/docs/gitglossary.html)

#### Creating a fork

1. Make sure you have a [github](github.com) account, and that you're signed in.
1. Navigate to the [Good Docs Project](https://github.com/thegooddocsproject), and click the repository you want to fork.
1. Click the `Fork` button in the top-right corner, and select the account you want to use.
1. Wait for github to create your fork and redirect you.
Take note of the repository you are now in, called `github.com/<your_username>/incubator`.

When you have created the fork, you can clone the code to your local machine.

#### Cloning the code

1. Create a directory on your local filesystem to keep your work in.
You can call it anything you like, but most people use `workspace` or something similar.
1. In your browser, go to the github page for your fork.
The URL will be `github.com/<your_username>/incubator`, or you can get to it by clicking on your user image from the main github page, and selecting `Your repositories`.
1. Click the green `Code` download button, and copy the URL in the drop-down box.
1. Open a terminal on your local machine, make sure you are in your `workspace` directory, and clone the URL you copied.
Depending on how big the repository is, it could take some time to download.

   ```bash
   > cd ~/workspace
   > git clone https://github.com/<your_username>/incubator.git
   ```

When you have the code downloaded, you need to set the upstream repository.
This is important so that you can keep your local fork updated.

#### Setting the upstream repository

1. In your terminal, navigate to the directory where you checked out the code:

   ```bash
   > cd ~/workspace/incubator
   ```

1. Check out the `master` branch:

   ```bash
   > git checkout master
   ```

1. List the current remote branches:

   ```bash
   > git remote -v
   ```

   This command should list two remotes, both marked `origin`, like this:

   ```bash
   origin  https://github.com/<your_username>/incubator.git (fetch)
   origin  https://github.com/<your_username>/incubator.git (push)
   ```

1. Add the incubator repo as an upstream:

   ```bash
   > git remote add upstream https://github.com/thegooddocsproject/incubator
   ```

1. Check:

   ```bash
   > git remote -v
   ```

   This command should now have the same two `origin` remotes as before, plus two more labelled `upstream`, like this:

   ```bash
   origin  https://github.com/<your_username>/incubator.git (fetch)
   origin  https://github.com/<your_username>/incubator.git (push)
   upstream  https://github.com/thegooddocsproject/incubator (fetch)
   upstream  https://github.com/thegooddocsproject/incubator (push)
   ```

Now that you have your repository set up, you can create a branch to work on.

#### Creating a branch

1. In your terminal, navigate to the directory where you checked out the code:

   ```bash
   > cd ~/workspace/incubator
   ```

1. Fetch the branches in the upstream repository:

   ```bash
   > git fetch upstream
   ```

1. Check out your fork's `master` branch:

   ```bash
   > git checkout master
   ```

   This will show a message like this:

   ```bash
   Switched to branch `master`
   ```

1. Merge the changes from the upstream `master` branch, into your fork's `master` branch:

   ```bash
   > git merge upstream/master
   ```

   This shows some output that indicates what changes have merged in to your fork.
1. Create a new branch for the work you want to do.
   Make sure you give it an appropriate name, and include your username:

   ```bash
   > git checkout -b update-readme-username
   ```

Make your changes.
When you have finished, save your changes, and create a pull request.

Each branch and pull request must contain a single piece of work.
For example, if you want to update a particular page and fix some typos across a lot of different pages, create a branch for the page update, make the changes, and do a pull request.
Then create a new branch for the typos, and do a second pull request.
This makes it easier for you to track your own work, and also for reviewers looking at your pull requests.

#### Creating a pull request (PR)

1. Save your changes in your text editor.
1. In your terminal, add the changes to your commit:

   ```bash
   > git add .
   ```

   Don't forget the period at the end of this command!
1. Commit the changes, and provide a short description of what's in the commit:

   ```bash
   > git commit -m "Updated README file"
   ```

1. Push the changes to your fork:

   ```bash
   git push
   ```

1. In your browser, go to your fork on github.
   The URL is in the form `github.com/<your_username>/incubator`, or you can get to it by clicking on your user image from the main github page, and selecting `Your repositories`.
   In the banner at the top of the page, click `Compare and Create Pull Request`.
1. Give your PR a title, and write a description of the changes.
   Link any relevant issues, and tag people you want to review your changes.
   If you intend to add more commits to your PR, mark your PR as a draft so that reviewers know you have not finished.

## Choosing something to work on

This section discusses how to find something to work on within the Good Docs Project.

### Issues

Like most open source projects, there are always tasks to do.
For the list of issues, see [https://github.com/thegooddocsproject/templates/issues](The Good Docs Project template issues).
Look for issues with a `good first issue` tag if you want something small to start on.

When you have found an issue you want to work on, either assign the issue to yourself, or leave a comment stating that you are going to work on it before you get started.
Add comments in the issue to ask questions or to clarify requirements if you are uncertain.
When you have a pull request ready, link the issue in the pull request details, so that the issue closes when the PR merges.

### Reviewing pull requests

The entire community reviews pull requests from others.
The more reviews each pull request gets, the better the quality of our code.

Note that pull requests in different repositories within the Good Docs Project require different levels of review rigor.
For example, the `incubator` repo has a much lower standard of code quality than the `templates` repo.
For a full explanation of our review standards, see [insert.link.here].

### Moving out of the incubator

Work in the `incubator` repository moves to the `templates` repository when complete.
By this stage, you should have been interacting with the rest of the Good Docs Project community on a regular basis.
Discuss moving your work across at a meeting, or send a note to the mailing list, and one of the project administrators will prepare a pull request for the move.

## Expectations and responsibilities

This guide covers the more technical aspects of contributing the Good Docs Project.
You also need to know how to be a good community citizen.
Make sure you visit [https://thegooddocsproject.dev/community.html](The Good Docs Project Community) to understand the expectations and responsibilities of our community.
