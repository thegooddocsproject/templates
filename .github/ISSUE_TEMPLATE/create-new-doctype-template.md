---
name: Create new doc type template
about: For issues where a templateer needs to create a new doc type template.
title: Create {doc_type} template
labels: templates
assignees: ''

---
# Title
{Keep the title short, yet descriptive.
Here are some examples:
* Create a new {doc_type} template 
* Align the existing {doc_type} template to new contributing guidelines
* Include a quality checklist for the quickstart template }

## Before you begin
{Optional: In this section specify any pre-requisites, background knowledge that the templateer should know before working on a template.}

1. Join The Good Docs [slack workspace](https://thegooddocs.slack.com/). 
2. Familiarize yourself with basic Git commands and understand the workflow for contributing on GitHub.
3. Read the [template contributing process](https://github.com/thegooddocsproject/templates/blob/dev/CONTRIBUTING.md#overview-of-the-template-writing-phases).
4. You are also strongly encouraged to join one of the [working groups](https://thegooddocsproject.dev/working-group/) to get valuable support from the community.

## Description
{Provide specific details about the template. You could adopt a user story approach to describe a new {doc_type} template.  

_As a [type of user] I want [my goal] so that [my reason]._  

Example:
_As a developer, I want an installation template to document the install instructions for my application._ 

Keep the following points in mind while writing the description:
* If applicable, always include the relevant people using `@{Username}` who can support in resolving the issue. It can be someone who has previously worked on the template. Also, indicate the relevant slack channel where the templateer can reach out to the larger community. 
* Use bullet points and subheadings to structure complex details instead of big paragraphs.
* Add links to any document references.
}

### Doc Type Name: {doc_type}

### Directory: https://github.com/thegooddocsproject/templates/{directory_name}

## Tasks
{Optional: Specify a broad list of tasks to help the templateer get started with the template.}
1. Research examples and identify best practices for writing a {doc_type}.
2. Create {doc_type}-template.md and write content for it.
3. Create {doc_type}-template-guide.md and write content for it.

## Helpful Resources
{Optional: Add links to anything that might help the templateer write this particular type of template. For example, a Medium article about how to write good tutorials.}
* [Template deliverables] (https://github.com/thegooddocsproject/templates/blob/dev/template-deliverables.md)
* [Template roles and resources] (https://github.com/thegooddocsproject/templates/blob/dev/template-roles-and-resources.md)
  
## Before you submit
Add an appropriate label to denote the relative priority of this template:

Label | Description
--|--
`templates-p0`| Base template, required to start other templates
`templates-p1` | 1.0 MVP alpha release: Key doctypes that authors need help with.
`templates-p2` | 2.0 Common doctypes used within open source.
`templates-p3` | 3.0 Comprehensive set of doctypes
`templates-p4` | 4.0 Special case doctype