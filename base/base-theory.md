# {Doctype} theory

This {doctype}-theory document provides reasoning, justifications, and links to research relevant to {doctype} documentation. It aims to:
* Advise a docset-owner in how to right size a {doctype}-template and {doctype}-guide for a project.
* Empower authors to "think like a tech writer and expert in {doctype} documents" and make decisions backed by best practices.

**Version:** {MAJOR.MINOR.PATCH}

**Last updated:** {Month DD, YYYY}

## User stories

{Tip:
* In selecting personas for user stories, you should make use of default Good Docs personas. (TBD: We need to define create this list.)

}

When writing, it is important to understand who you are writing for, and ensure that you provide just the right amount of information to address their needs. The following user stories should help you achieve that.

A {doctype} document aims to address the following user stories:

* As a {user persona}, I want to {achieve a specific goal}, so that I can {achieve a larger business objective}.
* ...

For a description of common personas, refer to 
_{TBD: We should link to a page we are yet to write helping people pick personas.}_

## Nature of content

{Doctype} documentation is {Discuss the nature of the content for this doctype:

* Discuss what format will best express the nature of the content. For example, text only, or multi-media options such as diagrams, screenshots or video.
* Discuss how the format you choose will impact maintenance. This can include human work-hours, as well as ongoing processes and infrastructure requirements.
* Reference your style guide, which should have recommended guidelines for using multimedia, such as image size and video length.
* For content with numerous items or steps, consider "chunking" content into sub-sections of 5-10 steps. It makes the information easier to read and remember, and gives the reader a sense of accomplishment after each chunk is completed. Chunking is recommended by major companies, such as Microsoft in its [writing style guide](https://docs.microsoft.com/en-us/style-guide/procedures-instructions/writing-step-by-step-instructions#complex-procedures), and from the Nielsen Norman Group's [research on chunking and usability](https://www.nngroup.com/articles/short-term-memory-and-web-usability/).

}

## Priorities for each quality criteria

* Each `doctype` addresses different use cases. It targets different user personas, with different needs.
* As such, there are different weightings applied to quality characteristics for each `doctype`. Reference documentation needs to comprehensively address all the features in the latest version, but can tolerate lower quality writing. Tutorials likely need only cover a sample of use cases, for an older version of the software, but there is a greater need for writing quality.
* The following table is used to help prioritize your time when writing for this {doctype} doctype.


|Quality criteria                                        |Priority to address                                                                |
|:-------------------------------------------------------|:----------------------------------------------------------------------------------|
|Currency: Alignment with the latest version of software.|{Select one of: Must, Should, Nice to have (May), Not Applicable (N/A), Should not}|
|Currency: Alignment with a specified version of software.|                                                                                  |
|Comprehensive: Covers every feature and use case.       |                                                                                   |
|Well written: Unambiguous.                              |                                                                                   |
|Well written: Concise, high information density.        |                                                                                   |
|Well written: Aligns with writing style guide.          |                                                                                   |
|Well written: Engaging, entertaining, draws the reader in.|                                                                                 |
|Audience: Target a specific persona and user story. Simplifies documentation by assuming prerequisite knowledge of the audience.|           |
|Audience: Targets a broad international, multicultural audience. Avoids slang, colloquialisms, pop cultural references or local references.||
|Audience: Considers a non-English speaking audience. Uses simple English.|                                                                  |
|Audience: Consider accessibility and disability in audiences.|                                                                              |
|Audience: Consider diversity and inclusiveness in language chosen.|                                                                         |
|Maintainability: Written to be easily translated.        |                                                                                  |
|Maintainability: Uses timeless language with reduced need to update over time.|                                                             |
|Maintainability: Has established processes for auditing and updating content.|                                                              |
|Maintainability: Has a healthy, engaged community of contributors.|                                                                         |

Note: The terms "Must”, "Should”, and "May” should be interpreted as per [RFC 2119](https://www.ietf.org/rfc/rfc2119.txt).

_TBD: The quality criteria list requires review and refinement._
* _Further reading: [Tom Johnson's article on Measuring Doc Quality](https://idratherbewriting.com/learnapidoc/docapis_measuring_impact.html)._
* _Further reading: Daniel Beck's Doc Audit work. TBD: Get the public link for this._

## Implementation strategy

{Tip:

* This section is optional.
* In some cases there may be tips you can provide on how to create a specific `doctype`.

}

## Customization

{Tip:

* There are often multiple approaches to consider when implementing a `doctype`.
* In this section you should discuss different approaches that can be applied to this `doctype`, including logic and recommendations to help a docset owner select the best strategy for them.
* Often there would be a light and more comprehensive version of this template. Immature projects may only have the capacity to maintain the light version. You should discuss how a project might mature their docs from light to comprehensive versions.

_{TBD: Add further guidance and sample text here.}_

_{TBD: We are encouraging docset owners to branch a template and then customize. This branched version now won't track latest updates to The Good Docs Project templates. A more sustainable approach would be to have an accompanying configuration file which supports section inclusion logic and variables. A future toolchain would need to be set up before we could introduce accompanying config files.}_

There are multiple approaches which can be taken to customize this template. These may depend upon:
  * The maturity of your project.
  * The size, interest, and skillsets of your contributor community.
  * The documentation goals you have for the project.

This section discusses approaches you may take to customize this template to your project.

{Tip:

* {Add customization advice here. …}

}

## Maintenance strategy

See also the maintenance strategy section of the `doctype_guide`.

{Tip:

* In this section, you should recommend strategies for maintaining `doctype` documentation. This could include:
* Automated documentation generation from code.
* Automated reports which highlight:
    * When documentation is out of date with software.
    * When documentation hasn’t been reviewed for a while.
* Integrating documentation checklists into software deployment, build, and test processes.
* This section can remain empty if there are no extra recommendations to add beyond general guidance in the `doctype_guide`.

}

## Backing research and further reading

{Tip:

It isn’t sufficient to simply define best practices for a `doctype`. You should provide compelling evidence as to why this is the best approach. If there isn't any research, then say so, provide your own recommendations, and explain why you think they are the best approach.

"Do the hard work to make it simple." [UK Open Government Design Principle](https://www.gov.uk/guidance/government-design-principles#do-the-hard-work-to-make-it-simple)

}

This section should summarize competing approaches and explain why you took the chosen approach.
* It might also suggest situations where a docset owner would select a different approach.
* Authoritative sources should be provided to justify recommendations.
* If this section becomes more than a page long, consider extracting out into a separate research paper and then reference the paper.

}

## Specific sections

This section discusses background theory associated with specific sections within {doctype} sections.

### Metadata

TBD: This content should move into a Docset Owner's guide.

The metadata fields which should be included in a document depends upon:
* The value the metadata field provides to the target audience for the doctype.
* The project's capacity to collect and maintain the metadata field. Can it be collected automatically?
* The maturity and quality criteria set for the project.

**Note:** Be careful not to overcommit to the number of metadata fields you introduce into your project's documentation:
* Many metadata fields need to be maintained manually which adds a maintenance burden to the project.
* If any of the metadata on a site is inaccurate or dated, it will reduce the trustworthiness of all content on the site, as the user typically won’t be able to determine which of the content is trustworthy.
* As such, a project should only adopt metadata fields which are automatically maintained by your documentation publishing system, or where there is an established, low-effort process to ensure the metadata is maintained.

Use the following table to help select the metadata fields to include in your {doctype} template:

|Metadata field    |schema.org name|Typical location in doc         |Priority - startup|Priority - mature|
|:-----------------|:--------------|:-------------------------------|:-----------------|:----------------|
|Title             |name           |\<title> and \<h1> heading      |Must              |Must             |
|Description       |description    |First paragraph summary         |Must              |Must             |
|Doc version       |version        |Front metadata list             |May               |Should           |
|Doc publish date  |datePublished  |Front metadata list             |Must              |Must             |
|Reading time      |-              |Front metadata list             |May               |May              |
|Target app version|-              |Front metadata list or Footer   |May               |Should           |
|License           |license        |Footer                          |Should            |Must             |
|Target audience   |audience       |Within first paragraph summary  |May               |Should           |

**Note:** The terms "Must”, "Should”, and "May” should be interpreted as per [RFC 2119](https://www.ietf.org/rfc/rfc2119.txt).

_(TBD: Discuss/improve recommendations for [schema.org](https://schema.org/) metadata fields. The table above should cover all metadata fields we consider should be recommended in the The Good Docs Project.}_

### Machine readable structured metadata

* TBD: This content should move into a Docset Owner's guide.
* TBD: Make sure the terms selected align with https://www.w3.org/TR/json-ld11/

To improve the searchability of your website, mature documentation projects should introduce machine readable, structured metadata. Refer to Google's [Understand how structured data works](https://developers.google.com/search/docs/advanced/structured-data/intro-structured-data).

Structured metadata is typically applied by embedding [JSON-LD](http://json-ld.org/) snippets into your documents, such as:

```javascript
<!--Machine readable schema.org structured metadata about this document.-->
<script type="application/ld+json">
{
  "name": "{Title of the document}",
  "description": "{Copy of the summary text}",
  "version": "{MAJOR.MINOR.PATCH}"
  "datePublished": "{Month DD, YYYY}",
  "license": "{URL to license}",
  "audience": "{Persona you are writing for, such as: developer, business manager, …}"
}
</script>
```

## The Revision history section

__This section typically should not be included. It is typically only included for formal documents where readers are likely to be interested in the document's change history.__

__It typically should only list major, public facing updates.__

__If included, it should follow the following format:__

The following table describes the history of {all/major} decisions and revisions made to this {document} over time. 

This guide uses the Major.Minor.Patch [semantic versioning](https://semver.org/) convention.

Edition|  Date        |Lead Author(s)  |Link to Repository Commit/Tag
-------|  ----        |--------------  |-----------------------------
0.2    |  {YYYY-MM-DD}|{Your name here}|Customised for this project's needs
0.1    |  {YYYY-MM-DD}|{Your name here}|Initial [{doctype}-template {version}](https://github.com/thegooddocsproject/templates/tree/main/{doctype}) from The Good Docs Project.


## The Decision log section

__This section typically should not be included, or should be included in an accompanying document.__

__It is typically only included for business process documents where readers may challenge the reasoning behind a decision.__

__If included, it should follow the following format:__

The following table describes the history of all decisions made to this {document} over time:

Ref  |  Date         |  Description                               |  Agreed to by
---  |  ----         |  -----------                               |  ------------
1    | {YYYY-MM-DD}  |  {Explain the decision that was made here} |  {Name or role}

## Acknowledgements

* This section is optional.
* Here you can acknowledge source material, and organizations or people who have contributed to this document.
