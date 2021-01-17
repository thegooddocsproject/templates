# About Base Template

{Template author tip:

* This about-base-template captures the structure and common elements that all downstream about-xxx-templates should follow.
* It provides guidance for both template authors as well as document authors.
* "Template author and template reviewer tips” should be removed from the final about-{doctype}-template.md. Other tips should remain.
* adjust other tips to align with the doctype you are writing for.

}

This document provides guidance related to the authoring of documents based on the {doctype}-template. It focuses on the "how”, "why” and where applicable, references background theory to justify the approaches recommended.

## Introduction

_{TBD: Introduction text below needs adjusting to align with revised base template structure.}_

This document is a base template that you can use to create any other template. The base template guides you through the steps to create a functional template that can be reused, adhered to, and followed consistently throughout.

Using a well-defined template helps to maintain consistency and integrity across all documentation while simplifying the process of creating any required document. It can save you time and effort, while ensuring consistency, clarity, and uniformity across your documentation suite.

The base template goes one step further, in that it helps you create any template for a given document type. It gives you direction in building the required template for a specific use case.


## Prerequisites

To make the best use of this guide, you should have a working knowledge of:

* [Git](https://git-scm.com/): The version control system used.
* [GitHub](https://github.com/thegooddocsproject): The project hosting platform used, along with associated project management tools.
* [GitHub Flavored Markdown](https://github.github.com/gfm/): The markup language used to write template documentation.
* [Currently implemented doctypes templates](https://github.com/thegooddocsproject/templates): To help identify if you need to create a new template or edit an existing one.
* Technical writing: To produce a well-written document that includes the relevant references.

## Target audience for templates

The templates target multiple audiences. They include writing tips for the following roles:


### Template author

{Template author tip: Remove this "template author” section from about-{doctype}-template.md files.}

A template author creates a new template in line with base and core templates.


### Template reviewer

{Template author tip: Remove this "template reviewer” section from about-{doctype}-template.md files.}

A template reviewer reviews the new template against template guidelines.


### Template customizer

A template customizer customizes a doctype template to align with a specific project or organizational guidelines. For example, specify the style guide to use with the template.


### Docset owner

A docset owner establishes an Information Architecture and Documentation Management Plan for a project. Typical tasks include:

* Select a set of doctype templates for the project.
* Customize templates if needed.
* Select a style guide for the project.
* Establish the docset maintenance process.

A docset owner should capture documentation decisions within a Documentation Management Plan.

_{TBD: We should define a template for a Documentation Management Plan, then reference from here.}_

The [Information Architecture Guide](https://thegooddocsproject.dev/ia-guide.html) aims to help docset owners with some of these tasks.

### Document author

A document author writes content in line with templates. Typically the document author is a subject matter expert and not a dedicated technical writer.

Ideally, their document will receive feedback and guidance from a document reviewer and/or their docset owner.

### Document reviewer

Documentation is almost always improved when it is reviewed against the doctype’s template, the selected style guide, writing best practices and is reviewed for technical accuracy. While not essential, it helps if one of the reviewers is a dedicated technical writer.

### Document reader

And of course, we need to understand the needs of the final document reader. There are likely multiple reader personas to consider, which depends upon the reader’s role, their technical expertise, their specific goal, and so on.

## Inheritance of template sets

There is a hierarchy of inheritance between template documents.

_{TBD: Insert hierarchy diagram here.}_

### Base (abstract) template set

The base template describes common features which are to be inherited by all doctype templates.

**Target audience:** Template authors.

**Documents:**

* base-template.md: Provides common structure, elements and writing tips for downstream xxx-template.md files.
* about-base-template.md: Provides common structure, elements and writing tips for downstream about-xxx-template.md files.

### Core (abstract) templates set

Each core template describes a group of template characteristics inherited by other doctype templates. Examples include Concept, Task, and Reference templates.

Core templates inherit from the base template.

**Target audience:** Template authors

**Documents:**

* xxx-template.md: Common structure, elements, and writing tips for downstream xxx-template.md files.
* about-xxx-template.md: Common structure, elements, and writing tips for downstream about-xxx-template.md files.

### Doctype templates set

Doctype templates provide instructions for writing content for a specific doctype.

Doctype templates inherit from a core or base template.

**Target audience:** Document authors, document reviewers, docset owners.

**Documents:**

* {doctype}-template.md:
    * Provides document headings, structure, common text, and specific writing tips for a specific &lt;doctype>.
    * Writing tips focus on the "what” to include and not the "how”, "why”.
* about-{doctype}-template.md:
    * Provides further guidance related to the use of the template. It focuses on the "how”, "why” and where applicable, references background theory. It covers topics like:
        * The target audience for this doctype.
        * Checklists of goals to achieve.
        * Priorities of different quality metrics for this doctype.
        * How the template might be customized.
        * When you would or would not use this doctype-template.
* Example-{doctype}.md:
    * A more comprehensive example of the template, describing the fake chronologue example project. _{TBD we haven’t finished defining this fake project yet.}_

### Documents

Documents are written to align with the Doctype templates.

**Target audience:** Readers (broken down by personas).

**Document:**

* {final-document}.md

## Microcontent

_TBD: We need to decide on the correct term to use between: structured data, microcontent, micro-content, microdata, snippets, metadata._

* _Microcontent_
    * _This is quite an evocative term._
    * _I [notice](https://www.youtube.com/watch?v=CoShm-AXYP4&list=PLZAeFn6dfHpl2E5JhVd34llZD4a4oAeCo&index=19) Scott DeLoach is using the term "microcontent", but haven’t seen that term used elsewhere._
    * _Searching "microcontent” in Google doesn’t find an authoritative definition._
* _Microdata:_
    * _Also evocative of the meaning._
    * _Probably don’t use [microdata](https://www.w3.org/TR/microdata/), which is the term used for a specific W3C implementation for structured data._
* _[Structured data](https://developers.google.com/search/docs/guides/intro-structured-data):_
    * _Term is used by Google._
    * _But isn’t as evocative as "microcontent”_
    * _Doesn’t have a wikipedia entry_

{Template author tip: All templates for The Good Docs Project must describe recommended [structured data](https://developers.google.com/search/docs/guides/sd-policies) fields. Fields selected should align with equivalent doctypes used in [schema.org](https://schema.org/).}

Microcontent fields are machine readable snippets of [structured data](https://developers.google.com/search/docs/guides/sd-policies) which describe their associated page. It is typically presented as concise text or an image.

All technical documentation should include microcontent. It helps search engines index pages appropriately, and facilitates content reuse.

Within The Good Docs Project, we have adopted the [JSON-LD](http://json-ld.org/) format for microcontent, [as recommended by Google](https://developers.google.com/search/docs/guides/intro-structured-data).

Note:

* Many microcontent fields need to be maintained manually which adds a maintenance burden to a project.
* If any of the microcontent on a site is inaccurate or dated, it will reduce the trustworthiness of all the microcontent on the site, as the user typically won’t be able to determine which of the content is trustworthy.
* As such, a project should only adopt microcontent fields which are automatically maintained by your documentation publishing system, or where there is an established, low-effort process to ensure the microcontent is maintained.

## Primary goal

{Template author tip: Concisely state the primary purpose of this doctype, ideally in one short sentence.}

## Target audience and user stories

{Template author tip: You should document the key user stories that this template is likely to be used for.}

{Docset owner tip: Select the user stories which are applicable to your project.}

This {doctype} template aims to address the following user stories:

* As a {user persona}, I want to {achieve a specific goal}, so that I can {achieve a larger business objective}.

{Template author tip: You may optionally add a "docset owner tip” explaining when the following user story should or should not be included.}

* As a {user persona}, I want to {achieve a specific goal}, so that I can {achieve a larger business objective}.
    * {Docset owner tip: Include this user story when … .}

## Nature of content

{Template author tip: 

* Discuss the nature of the content for this doctype.
* Decide what format will best express the nature of the content. For example, text only, or multi-media options such as diagrams, screenshots or video.
* Consider how the format you choose will impact maintenance. This can include human work-hours, as well as ongoing processes and infrastructure requirements.
* Reference your style guide which should have recommend guidelines for using multi-media such as image size and video length.

}

## Priorities for each quality criteria

{Template author tip: 

* Each doctype addresses different use cases. It targets different user personas, with different needs.
* As such, there are different weightings applied to quality characteristics for each doctype. Reference documentation needs to comprehensively address all the features in the latest version, but can tolerate lower quality writing. Tutorials need only cover a sample of use cases of an older version of the software, but there is a greater need for writing quality.}

{Docset owner tip: Select the quality criteria which will be important for your project.}

This table lists the relative importance of the following quality criteria for {doctype} documents.


|Quality criteria|Priority to address|
|--- |--- |
|Currency: Alignment with the latest version of software.|{Select one of: Must, Should, Nice to have (May), Not Applicable (N/A), Should not}|
|Currency: Alignment with a specified version of software.||
|Comprehensive: Covers every feature and use case.||
|Well written: Unambiguous.||
|Well written: Concise, high information density.||
|Well written: Aligns with writing style guide.||
|Well written: Engaging, entertaining, draws the reader in.||
|Audience: Target a specific persona and user story. Simplifies documentation by assuming prerequisite knowledge of the reader.||
|Audience: Targets a broad international, multicultural audience. Avoids slang, colloquialisms, pop cultural references or local references.||
|Audience: Considers a non-English speaking audience. Uses simple English.||
|Audience: Consider accessibility and disability in audiences.||
|Audience: Consider diversity and inclusiveness in language chosen.||
|Maintainability: Written to be easily translated.||
|Maintainability: Uses timeless language with reduced need to update over time.||
|Maintainability: Has established processes for auditing and updating content.||
|Maintainability: Has a healthy, engaged community of contributors.||

Note: The terms "Must”, "Should”, and "May” should be interpreted as per [RFC 2119.](https://www.ietf.org/rfc/rfc2119.txt) 

_TBD: The quality criteria list requires review and refinement._
_TBD: Further reading: [Tom Johnson's article on Measuring Doc Quality](https://idratherbewriting.com/learnapidoc/docapis_measuring_impact.html)._

## Implementation strategy

{Template author tip:

* This section is optional.
* In some cases there may be tips you can provide on how to create a specific doctype.

}

## Customization

{Template author tip:

* There are often multiple approaches to consider when implementing a doctype.
* In this section you should discuss different approaches that can be applied to this doctype, including logic and recommendations to help a docset owner select the best strategy for them.
* Often there would be a light and more comprehensive version of this template. Immature projects may only have the capacity to maintain the light version. You should discuss how a project might mature their docs from light to comprehensive versions.

_{TBD: Add further guidance and sample text here.}_

}

{Docset owner tip:

* There are multiple approaches which can be taken to customize this template. These may depend upon:
    * The maturity of your project.
    * The size, interest, and skillsets of your contributor community.
    * The documentation goals you have for the project.
* This section discusses approaches you may take to customize this template to your project.

}

{Template author tip:

* Add content here. …}

}

## Maintenance strategy

The long term health of documentation depends upon the project's ability to establish sustainable maintenance processes for each doctype.

* If content on a site is inaccurate or dated, it will reduce the trustworthiness of all the content on the site, as the user typically won’t be able to determine which of the content is trustworthy.
* As such, a project should only create content where there is commitment for continued maintenance of the content.

This section suggests maintenance strategies which can be applied for {doctype} documents.

{Docset owner tip:
*  You should select and set up an appropriate strategy for maintaining {doctype} documents. This strategy should be described in your Documentation Management Plan.

}

_{TBD: We should define a template for a Documentation Management Plan, then reference from here.}_

{Template author tip:

* In this section, you should recommend strategies for maintaining {doctype} documentation. This could include:
* Automated documentation generation from code.
* Automated reports which highlight:
    * When documentation is out of date with software.
    * When documentation hasn’t been reviewed for a while.
* Integrating documentation checklists into software deployment, build, and test processes.

}

## Business case

{Template author tip:

* In this section, discuss strategies to calculate the cost of implementing this doctype. This may just be to reference the Development strategy and Maintenance strategy above.
* Then suggest business goals and reasons why this doctype would help address these goals. Business goals might be:
    * Increased developer efficiency.
    * Faster onboarding for users and/or developers.
    * Reduced support costs.
* Consider the case where the docs are only partially maintained. Would it be better to have no documentation than incorrect or partially maintained documentation?

}

### When to include {doctype} docs?

{Template author tip:

* Add a summarized list of reasons for including the doctype, based on the business case above. 

}

Include {doctype} docs if:

* {Reason 1.}
* {Reason 2.}

### When wouldn’t you include {doctype} docs?

{Template author tip:

* Add a summarized list of reasons for not including the doctype, based on the business case above. 

}

Don't include {doctype} docs if:

* {Reason 1.}
* {Reason 2.}

## Checklist

{Template author tip:

* Add checklist items which are specific to this doctype.

}

Before finalizing your {doctype} document, ensure you have addressed the following:

* The document has been reviewed:
    * For clear writing and alignment with the writing style guide, ideally by a technical writer or editor.
    * For alignment with the {doctype} template, ideally by a technical writer, information architect, or content strategist.
    * For technical accuracy, ideally by a technical subject matter expert.
* {Further checklist items ... .}

## Backing research and further reading

{Template author tip:

* It isn’t sufficient to simply define best practices for a doctype. You need to provide compelling evidence as to why this is the best approach. This section should summarize competing approaches and explain why you took the chosen approach.
* It might also suggest situations where a docset owner would select a different approach.
* Authoritative sources should be provided to justify recommendations.
* If this section becomes more than a page long, consider extracting out into a separate research paper and then reference the paper.

}
