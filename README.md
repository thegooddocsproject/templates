# About the Templates Repo

This repository contains best-practice templates to help build documentation for open-source software, which incidentally is directly applicable to other domains too.

Here we provide tips for using these templates.

## Core documentation types

The templates are categorised in line with standard [DITA](http://docs.oasis-open.org/dita/dita/v1.3/errata02/os/complete/part3-all-inclusive/archSpec/technicalContent/dita-technicalContent-InformationTypes.html#dita_technicalContent_InformationTypes) documentation types:

**Concept**: Describes how and why things work.
Concepts are normally written to help the reader understand a technology, prior to using it.

**Task**: Gives specific instructions about how to get something done.
In practice, Tasks tend to have a specific goal and usually consist of a set of numbered steps that the reader can follow to achieve the goal.

**Reference**: Contains structured information or specifications that users need to make a product work.
Reference sections should comprehensively catalog data such as functions and their parameters, return codes and error messages.

Our templates follow these documentation types, and you should find that your information naturally fits into them as you write.

## How to use these templates

We like to compare documentation types to aisles in a grocery store.
Each aisle includes related templates, which you can think of as ingredients.
Use these ingredients in documentation cookbooks to whip up docs for your readers.

When writing your documentation, it helps to think about the following:

* Who are you writing for?
* What will they be trying to accomplish when they read the documentation?
* The information type. Is it a concept, a task or reference?

## The templates

Current templates:

| Template name | Documentation type | Description |
| ------------- | ------------------ | ----------- |
| API Project overview | Concept | An overview of your API |
| API Quickstart | Concept, Task | Simplest possible method of implementing your API |
| API Reference | Reference | List of references related to your API |
| Discussion | Concept | Longer document giving background or context to a topic |
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
