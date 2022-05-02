---
name: Create new content type template
about: For issues where a templateer needs to create a new content type template.
title: Create {content_type} template
labels: templates
assignees: ''

---
# Title
{Keep the title short, yet descriptive.
Here are some examples:
* Create a new {content_type} template 
* Align the existing {content_type} template to new contributing guidelines
}

## Before you begin
{Optional: In this section specify any pre-requisites or background knowledge that the templateer should know before working on a template.}

1. Join The Good Docs Project [slack workspace](https://thegooddocs.slack.com/). 
2. Read the [template contributing process](https://github.com/thegooddocsproject/templates/blob/dev/CONTRIBUTING.md#overview-of-the-template-writing-phases).
3. You are strongly encouraged to join one of the [working groups](https://thegooddocsproject.dev/working-group/) to get valuable support from the community such as mentorship, Git training, and helpful feedback as you contribute to your first template.
4. Request access to the `templates` repository by joining the #templates channel in slack and posting a request. 
5. Assign yourself to an issue for the template that you want to work on.
6. Add the issue to the [templates-kanban](https://github.com/thegooddocsproject/templates/projects/1) and move it into the `Research-phase` column.
7. While it is not mandatory to know Git to start contributing, if you are keen, you can familiarize yourself with basic git commands and understand the workflow for contributing on GitHub.  
:information_source: The template leads also provide free hands-on training on Git to the contributors on a need-basis.

## Template description
{Provide specific details about the template. You could adopt a user story approach to describe a new {content_type} template.  

_As a [type of user] I want [my goal] so that [my reason]._  

Example:
_As a developer, I want an installation template to document the install instructions for my application._ 

Keep the following points in mind while writing the description:
* If applicable, always include the relevant people using `@{Username}` who can support in resolving the issue. It can be someone who has previously worked on the template. Also, indicate the relevant slack channel where the templateer can reach out to the larger community. 
* Use bullet points and subheadings to structure complex details instead of big paragraphs.
* Add links to any document references.
}

### Content type name: {content_type}

### Directory: https://github.com/thegooddocsproject/templates/{directory_name}

## Tasks
{Optional: Specify a broad list of tasks to help the templateer get started with the template.}
1. Research examples and identify best practices for writing a {content_type}.
2. Create drafts of the template set deliverables.
3. Contact the template leads to let them know that your draft is ready for community review. 
4. Get feedback on the drafts from the community.
5. After making revisions, submit a pull request. 

## Helpful resources
{Optional: Add links to anything that might help the templateer write this particular type of template. For example, a Medium article about how to write good tutorials.}
* [Template Contributing Process] (https://github.com/thegooddocsproject/templates/blob/dev/CONTRIBUTING.md)
* [Template deliverables] (https://github.com/thegooddocsproject/templates/blob/dev/template-deliverables.md)
* [Template roles and resources] (https://github.com/thegooddocsproject/templates/blob/dev/template-roles-and-resources.md)
  
## Before you submit
Add an appropriate label to denote the relative priority of this template:

Label | Description
--|--
`templates-p0`| Base template, required to start other templates
`templates-p1` | 1.0 MVP alpha release: Key content types that authors need help with.
`templates-p2` | 2.0 Common content types used within open source.
`templates-p3` | 3.0 Comprehensive set of content types
`templates-p4` | 4.0 Special case content type