# About the Templates Repo

This repository contains best-practice templates to help build documentation for open-source software, which incidentally is directly applicable to other domains too.

Here we provide tips for using these templates.


## Core documentation types

The templates are categorized into three documentation types:

**Concept**:
Describes how and why something works.
Concepts answer the question "what is it?".
When readers read concepts, they are learning about a topic.
Use concepts to help the reader understand a technology, before they start using it.

**Task**:
Gives specific instructions about how to get something done.
Tasks answer the question "how do I do it?".
When readers read tasks, they are doing something.
Tasks tend to have a specific goal and consist of a set of numbered steps that the reader can follow to achieve that goal.

**Reference**:
Contains structured information or specifications that users need to make a product work.
Reference material answers the question "what else do I need to know?"
When readers read references, they are fact-checking.
Reference sections should comprehensively catalog data such as functions and their parameters, return codes and error messages.
They are often presented as tables, bulleted lists, or sample scripts.

Our templates follow these documentation types, and you should find that your information naturally fits into them as you write.


## How to use these templates

We like to compare documentation types to aisles in a grocery store.
Each aisle includes related templates, which you can think of as ingredients.
Use these ingredients in documentation cookbooks to whip up docs for your readers.

When writing your documentation, it helps to think about:

* Who are you writing for?
* What will they be trying to do when they read the documentation?
* What information are you providing? Is it a concept, a task, or reference?


## The templates

Current templates:

| Template name | Documentation type | Description |
| ------------- | ------------------ | ----------- |
| API Project overview | Concept | An overview of your API |
| API Quickstart | Concept, Task | Simplest possible method of implementing your API |
| API Reference | Reference | List of references related to your API |
| Explanation | Concept | Longer document giving background or context to a topic |
| How-to | Task | Short series of steps for a particular task |
| Tutorial | Concept, Task | A training document for a product or topic |
| General reference entry | Reference | Specific details about a particular topic |
| Logging reference | Reference | Description of log pipelines |

## The cookbook

| Recipe name | Description |Constituent templates |
| ------- | ------- | ----------------- |
| API reference | One chapter in your full API documentation | Reference entries (multiple reference) + error information (reference) + throttling (concept) + authentication (task) |
| API guide: good | The starter set for API docs | API project overview + setup instructions (task) + Reference section (see recipe above) + Quickstart |
| API guide: better | Improved API docs, after learning about users | API project overview + setup instructions (task) + Reference(s) + Quickstart + How-to(s) |
