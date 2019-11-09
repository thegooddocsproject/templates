# About the Templates Repo

Everything you need to know to build documentation from these templates. 

## The three information types
The templates here are generally divided into three categories, and each template will tell you the category it belongs in. You've probably seen these before: The categories are based on information types that are often applied to technical information.

**Concept**
: Describes how and why things work. Concepts are normally written to help the reader with understanding a technology, prior to using it. 

**Task**
: Gives specific instructions about how to get something done. In practice, Tasks tend to have a specific goal and usually consist of a set of numbered steps that the reader can follow to achieve the goal. 

**Reference**
: Contains structured information or specifications that users need to make a product work. Reference sections tend to exhaustively catalog data such as error messages, return codes, or endpoints and their parameters.

There's a guideline in technical writing that most information falls into one of these categories, and that the information types need to be consolidated as much as possible, rather than mixed together. It makes sense to categorize the templates according to these types, because your writing most likely calls for chunks of information that can be categorized this way.

When writing your documentation, it helps to think about the following.

* Who you are writing for
* What they will be trying to acomplish when they read the documentation
* The information type. Is it a concept, a task or reference? 

On the last point, it's best not to add *a lot* of conceptual or task-based information in the middle of your API reference section; however, do make common sense adjustments such as adding comments (which are sort of conceptual) after your examples in an API reference.

## How to use these templates

We like to compare the three template types to aisles in a grocery store. The templates they contain are ingredients that you can combine to create your documentation. You'll definitely need more than one template to build your full set of documentation. You'll aso need to think about the recipes that you use to combine these ingredients into effective documentation. 

## The templates

Here are the templates we currently offer. (More to come soon.)

| Template name | Type |
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
| API guide: good | The starter set for API docs | API project overvew + setup instructions (task) + Reference section (see recipe above) + Quickstart |
| API guide: better | Improved API docs, after learning about users | API project overvew + setup instructions (task) + Reference(s) + Quickstart + How-to(s) |



