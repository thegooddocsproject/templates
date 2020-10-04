# Contributors' Guide

## Welcome to The Good Docs Project

The Good Docs Project provides a set of templates and other resources to help you create great documentation.
Anyone can come and make use of those resources, download the templates, and create their own documentation at any time.
If you have a great idea for improving any of the resources, we would love for you to share them!
This guide is to help you get started contributing to the Good Docs Project, whether you intend to contribute a whole new template to the collection, or fix a typo.

## Getting Familiar with the Project Repositories

All the source code for the Good Docs Project live in github, including the code for the website, examplar project, community governance, and the templates themselves.
Browse the code by navigating to [https://github.com/thegooddocsproject/] in your browser.

The Good Docs Project has a lot of repositories within it, and they all serve an individual purpose.
To contribute to the templates, there are two main repositories that you will need to work with, the `templates` repo, and the `incubator` repo.

### The `templates` repository

This is the main repository in the project, because it contains the templates, and their companion guidance documents.
If you want to make a small change to an existing template, such as updating some wording, or fixing a typo, you can propose a change directly within this repository.
Instructions on how to do that are later on in this guide.

### The `incubator` repository

The `incubator` repository is where we work on bigger projects, including new templates, before they are ready to go into the `templates` repository.
If you want to contribute a new template, or a larger piece of work for any other repository, this is the place to start.
When you propose a change to the `incubator` repo, you can work on it in collaboration with the rest of the community, and move it into the appropriate location when complete.

## Setting up your work environment

To work on content within the Good Docs Project, regardless of which repo you are proposing changes to, or whether the change is big or small, you will need to set up your work environment.
The main thing you will need is a text editor.

### Selecting a text editor

There are a large range of text editors available, and people who work in text editors a lot will always have their favorites.
Because of this, it can be a little daunting trying to choose which one you like.

Some popular free text editors are [Atom](https://atom.io/) and [Visual Studio Code](https://code.visualstudio.com/).
They are both graphical editors, and include some convenient features like a file browser and a command prompt, so you can manage your entire workflow within the editor.

However, you don't need anything fancy for small changes.
Your operating system will provide a simple text editor by default, and these are a great place to start:

| Operating System | Editor   |
| ---------------- | -------- |
| Windows          | Notepad  |
| MacOS            | TextEdit |
| Linux - Gnome    | gedit    |
| Linux - KDE      | KWrite   |

Once you've gotten started with a basic editor, you'll have a better idea of what features you want in a more advanced editor.

### Working with git

Version control with git can be confusing at first.
Generally, you will only need a few commands to get started, and once you've done it once or twice, it will start to become second nature.
The important thing to remember is that if you get confused and you're not sure what to do, you can always delete what you have on your local machine and start again, without losing too much work.

You will need to create a fork of the repository you want to contribute to.
A fork copies the current state of the repository to your own project, so you can make your changes safely.
When you have made your changes, you can then propose the changes back to the original project in a pull request.
The community will review your pull request, and you can make more updates or changes as needed.
When everyone is happy with the changes, the pull request is merged, and your changes become part of the code.

We will be using the `incubator` repository for this example, but the method is the same for any of the other repositories.

#### Creating a Fork

1. Make sure you have a [github](github.com) account, and that you're signed in.
1. Navigate to the [Good Docs Project](https://github.com/thegooddocsproject), and click the repository you want to fork.
1. Click the `Fork` button in the top-right corner, and select the account you want to use.
1. Wait for github to create your fork and redirect you.
Take note of the repository you are now in.
It will be called `github.com/<your_username>/incubator`.

When you have created the fork, you can clone the code to your local machine.

#### Cloning the Code

1. Create a directory on your local filesystem to keep your work in.
You can call it anything you like, but most people use `workspace` or something similar.
1. In your browser, go to the github page for your fork.
The URL will be `github.com/<your_username>/incubator`, or you can get to it by clicking on your user image from the main github page, and selecting `Your repositories`.
1. Click the green `Code` download button, and copy the URL in the drop-down box.
1. Open a terminal on your local machine, make sure you are in your `workspace` directory, and clone the URL you just copied.
Depending on how big the repository is, it could  take a little while to download.
   ```
   > cd ~/workspace
   > git clone https://github.com/<your_username>/incubator.git
   ```

When you have the code downloaded, you need to set the upstream repository.
This is important so that you can keep your local fork updated.

#### Setting the upstream repository

1. In your terminal, navigate to the directory where you checked out the code:
   ```
   > cd ~/workspace/incubator
   ```
1. Check out the `master` branch:
   ```
   > git checkout master
   ```
1. List the current remote branches:
   ```
   > git remote -v
   ```
   This command should list two remotes, both marked `origin`, like this:
   ```
   origin  https://github.com/<your_username>/incubator.git (fetch)
   origin  https://github.com/<your_username>/incubator.git (push)
   ```
1. Add the incubator repo as an upstream:
   ```
   > git remote add upstream https://github.com/thegooddocsproject/incubator
   ```
1. Check that the upstream was added properly:
   ```
   > git remote -v
   ```
   This command should now have the same two `origin` remotes as before, plus two more labelled `upstream`, like this:
   ```
   origin  https://github.com/<your_username>/incubator.git (fetch)
   origin  https://github.com/<your_username>/incubator.git (push)
   upstream  https://github.com/thegooddocsproject/incubator (fetch)
   upstream  https://github.com/thegooddocsproject/incubator (push)
   ```

Now that you have your repository set up, you can create a branch to work on.

#### Creating a branch

1. In your terminal, navigate to the directory where you checked out the code:
   ```
   > cd ~/workspace/incubator
   ```
1. Fetch the branches in the upstream repository:
   ```
   > git fetch upstream
   ```
1. Check out your fork's `master` branch:
   ```
   > git checkout master
   ```
   This will show a message like this:
   ```
   Switched to branch `master`
   ```
1. Merge the changes from the upstream `master` branch, into your fork's `master` branch:
   ```
   > git merge upstream/master
   ```
   This shows some output that indicates what changes have been merged in to your fork.
1. Create a new branch for the work you want to do.
   Make sure you give it an appropriate name.
   It is usually good practice to include your username as well:
   ```
   > git checkout -b update-readme-username
   ```

You can now go ahead and make your changes.
When you have finished, save your changes, and create a pull request.

Always try to make sure that you just work on a single piece of work for each branch and pull request.
For example, if you want to update a particular page and fix some typos across a lot of different pages, create a branch for the page update, make the changes, and do a pull request.
Then create a new branch for the typos, and do a second pull request.
This makes it much easier for you to keep track of what is going on in your fork, and also for reviewers looking at your pull requests.

#### Creating a pull request (PR)

1. Make sure all your changes are saved in your text editor.
1. In your terminal, add the changes to your commit:
   ```
   > git add .
   ```
1. Commit the changes, and provide a short description of what's in the commit:
   ```
   > git commit -m "Updated README file"
   ```
1. Push the changes to your fork:
   ```
   git push
   ```
1. In your browser, go to your fork on github.
   The URL will be `github.com/<your_username>/incubator`, or you can get to it by clicking on your user image from the main github page, and selecting `Your repositories`.
   There will be  banner at the top of the page, click the `Compare and Create Pull Request` button on the banner.
1. Give your PR a title, and write a description of the changes.
   Make sure you link any relevant issues, and tag any people you want to review your changes.
   If you intend to add more commits to your PR, mark your PR as a draft so that reviewers know you haven't finished work yet.






## Choosing something to work on

Compellingly iterate premium testing procedures through effective web services. Collaboratively recaptiualize client-based leadership skills rather than adaptive initiatives. Distinctively synthesize customer directed markets after worldwide portals. Appropriately exploit revolutionary e-services without excellent content. Assertively unleash clicks-and-mortar leadership skills with 2.0 action items.

### Issues

Assertively enhance functional solutions for synergistic opportunities. Proactively expedite cross-media synergy whereas cutting-edge services. Appropriately embrace principle-centered leadership via leveraged infomediaries. Competently negotiate top-line products through 24/365 experiences. Professionally matrix goal-oriented processes and bleeding-edge experiences.

### Pull Requests

Phosfluorescently actualize economically sound alignments rather than quality synergy. Seamlessly negotiate value-added intellectual capital before equity invested applications. Intrinsicly re-engineer real-time total linkage and bleeding-edge total linkage. Monotonectally procrastinate multimedia based internal or "organic" sources vis-a-vis impactful outsourcing. Appropriately visualize cross-media quality vectors and backward-compatible vortals.

### Moving out of the incubator

Credibly supply holistic materials without resource maximizing convergence. Interactively revolutionize e-business content after interdependent expertise. Uniquely synergize prospective niche markets before cost effective meta-services. Phosfluorescently initiate distributed core competencies rather than virtual architectures. Compellingly harness client-centered users whereas client-centered process improvements.

## Expectations and Responsibilities

Interactively provide access to economically sound core competencies whereas team driven convergence. Collaboratively plagiarize value-added outsourcing with high-payoff infomediaries. Phosfluorescently cultivate efficient e-tailers without proactive mindshare. Interactively provide access to excellent e-markets with seamless collaboration and idea-sharing. Phosfluorescently seize go forward architectures rather than standards compliant alignments.

Link to further governance stuff ...


## Glossary

<!--Get this into alphabetic order-->

<dl>
    <dt>Fork</dt>
    <dd>A local copy of an upstream repository.
    Use a fork to safely make changes, then submit a pull request to merge your changes into the upstream repository.</dd>
    <dt>Upstream repository</dt>
    <dd>The repository that you want to make changes to.</dd>
    <dt>Pull Request</dt>
    <dd>A request to merge the changes you have made locally, into the upstream repository.</dd>
    <dt>Branch</dt>
    <dd>A copy of the code you are working on, where all your changes are stored.
    Always work on a branch, do not commit anything directly to `master` or `main`.</dd>
    <dt>Master</dt>
    <dd>The `master` or `main` branch is a special branch that is at the top of the repository.
    Always work on a branch, do not commit anything directly to `master` or `main`.</dd>
</dl>