# {Doctype} guide

This guide is the primary document a author should follow when writing a {doctype} document. Sections explain **how** to write the corresponding section in the {doctype}-template.

**Version:** {MAJOR.MINOR.PATCH}

**Last updated:** {Month DD, YYYY}

## About {Doctype}

{Doctype} documentation is {discuss the nature of the content for this doctype}.

## Before you start this guide

To make the best use of this guide, it helps if you have a working knowledge of:

* {The project's / The Good Doc Project's / Google's / Microsoft's/...} documentation style guide.
* Technical writing basics, such as taught in Google's [technical writer training courses](https://developers.google.com/tech-writing).`

* Refer to the:
  * [{doctype}-template]({doctype}-template). You will fill flesh out this skeleton.
  * [{doctype}-example]({doctype}-example) for a filled in template.
  * [{doctype}-checklist]({doctype}-checklist) to confirm you are done.
  * [{doctype}-theory]({doctype}-theory) to understand the broader picture.

## Content of your {doctype} document

The following sections describe how fill in specific template sections.

### The hero description
The hero description stands alone, just under the title. It is sometimes referred to as the "TL;DR statement", short for: Too Long; Dont Read" and is sometimes written as:
```
   TL;DR: {Hero description.}
```
We recommend against including the "TL;DR" acronym as some readers might not be familiar with it.

It should be very short so that a reader will naturally want to read it. Its purpose is to quickly help the reader decide whether they should read any further.

It should concisely explain what this document covers, and the type of person who will be interested in reading it. 

### The document version metadata
To enable consistency and traceability between cross-referenced documentation and software, all documentation should be versioned.

A versioning convention should be adopted. It is usually best to follow the widely adopted [semantic versioning](https://semver.org/) MAJOR.MINOR.PATCH convention.

### The last updated metadata

The ```last updated``` field refers to the documentation's publication date. Follow the date naming convention from your project's style guide, such as [Google style guide's date guidance](https://developers.google.com/style/dates-times).

Make sure you use an unambiguous date format. Note that 4/5/1900 could be:
* April 5, 1900 in the United States.
* 4 May, 1900 in England.

If adopting the short hand formatting, select the universal date format: ```YYYY-MM-DD``` or ```YYYY-MM```.

### The application versions metadata
Where applicable, the documentation should list the version, or range of versions, of the application(s) this documentation describes.

### Other metadata fields

{Tips for using this field}

### The indicative reading time metadata

Reading speed usually should not be included in fields. There are two lines of thought around including a ```reading time``` field.

Pros:
* It helps someone decide whether they have time to read the page.

Cons:
* It is hard to account for:
    * The range of technial expertise and reading speeds of readers.
    * The varying technical complexity of source material.
    * Multiple authors applying differing rules to assess reading time.
* It potentially makes slow readers feel inadequate and demotivated.
* Reading time is less applicable for some doctypes.

Guidelines for calculating reading time:
* Base estimates on the least experienced and slowest target reader.
* Typically assume a reading speed of 50 words per minute for technical material, and 200 words per typical business material. [ExecuRead reading speed source assessment](https://secure.execuread.com/facts/#:~:text=The%20average%20reading%20speed%20is,roughly%202%20minutes%20per%20page.).

_TBD: Provide better researched references and theory to this._

## {Sections and subsections}

* Include standard headings applicable for this template’s `doctype`.
* Where applicable, provide standard text for relevant sections.
* Include tips for doc authors.
* Some sections will be optional and so should include the "optional" tip to the doc author.

### The Overview section

TBD: We should revisit the scope of this description and align with the hero description.

If you have a long document, you may additionally include an __Overview__ section. It should only be included if you have extra information which is too verbose to include in the concise __Hero Paragraph__.

Within this section, summarize what the reader will achieve by reading the explanation article:

* Are you writing for developers or for managers?
* Are you writing for people who have a certain problem to solve?
* Are you writing for a particular industry or market segment?

Readers should already have read a concept about the topic in an About article. Ensure you link to the relevant About article in the overview.

## The Before you start section

This section prevents readers from getting halfway through a document and discovering that they need to go and read other documentation before they can continue. Prerequisites can include:
* Skills to become familiar with or training to complete,
* Articles or information to read,
* Technical dependencies such as an internet connection, specific software or a development environment.

Describe what the audience needs to know, or needs to have, before they attempt reading this document. By stating the requirements up-front, you prevent your readers from having a bad experience with your document. You can include links to procedures or information, or give useful pointers about how to get what they need.

This section is optional and should only be included if required.

## The Further information section

{Template author tip: Most `doctypes` should provide links to help a document author find related topics and next steps.}

This section is optional.

Think about the persona(s) of your reader, and consider what they might want to know next. 

Provide one to four links to more information. Links should be a logical next step to what has already been read.
  * Don't overwhelm your reader with too many choices. Just select the one link per option for the most likely next steps.
  * Consider {next steps, similar concepts, background theory}.

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
