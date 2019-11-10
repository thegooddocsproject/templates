# About the Templates Repo

This repository contains best practice templates to help build documention for open source software, which incidentally is directly applicable to other domains too.

Here we provide tips for using these templates.

## Core documentation types
The templates are categorised in line with standard [DITA](http://docs.oasis-open.org/dita/dita/v1.3/errata02/os/complete/part3-all-inclusive/archSpec/technicalContent/dita-technicalContent-InformationTypes.html#dita_technicalContent_InformationTypes) documentation types:

**Concept**: Describes how and why things work. Concepts are normally written to help the reader with understanding a technology, prior to using it. 

**Task**: Gives specific instructions about how to get something done. In practice, Tasks tend to have a specific goal and usually consist of a set of numbered steps that the reader can follow to achieve the goal. 

**Reference**: Contains structured information or specifications that users need to make a product work. Reference sections should comprehensively catalog data such as functions and their parameters, return codes and error messages.

Our templates follow these categorizations, and you should find your information naturally chunks this way.


## How to use these templates

We like to compare documentation types to aisles in a grocery store. Each aisle includes related templates, which you can think of as ingredients. Use recipes to mix templates and create targetted documentation sets for a specific scenarios.

When writing your documentation, it helps to think about the following:

* Who are you writing for?
* What will they be trying to accomplish when they read the documentation?
* The information type. Is it a concept, a task or reference? 

On the last point, it's best not to add *a lot* of conceptual or task-based information in the middle of your API reference section; however, do make common sense adjustments such as adding comments (which are sort of conceptual) after your examples in an API reference.

## The templates

Templates we currently offer:

| Template name | Documentation type |
| ---------------------- | ------- |
API Project overview | concept 
API Quickstart | task
API Reference | reference
Discussion | concept
How-to | task
Tutorial | task
General reference entry | reference
Logging reference | reference

## The cookbook

| Recipe name | Description |Constituent templates |
| ------- | ------- | ----------------- |
| API reference | One chapter in your full API documentation | Reference entries (multiple reference) + error information (reference) + throttling (concept) + authentication (task) |
| API guide: good | The starter set for API docs | API project overview + setup instructions (task) + Reference section (see recipe above) + Quickstart |
| API guide: better | Improved API docs, after learning about users | API project overview + setup instructions (task) + Reference(s) + Quickstart + How-to(s) |



