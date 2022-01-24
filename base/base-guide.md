# {Doctype} guide

This {doctype}-guide provides extra writing tips describing **HOW** to fill in each of the sections within the {doctype}-template.

**Version:** {MAJOR.MINOR.PATCH}

**Last updated:** {Month DD, YYYY}

## Prerequisites

To make the best use of this guide, it helps if you have a working knowledge of:

* {The project's / The Good Doc Project's / Google's / Microsoft's/...} documentation style guide.
* Technical writing basics, such as taught in Google's [technical writer training courses](https://developers.google.com/tech-writing).

## {Doctype} content
### Hero description
The hero description stands alone, just under the title. It is sometimes referred to as the "TL;DR statement", short for: Too Long; Dont Read" and is sometimes written as:
```
   TL;DR: {Hero description.}
```

We recommend against including the "TL;DR" acronym as some readers might not be familiar with it.

It should be very short so that a reader will naturally want to read it. Its purpose is to quickly help the reader decide whether they should read any further.

It should concisely explain what this document covers, and the type of person who will be interested in reading it. 

### Document version
To enable consistency and traceability between cross-referenced documentation and software, all documentation should be versioned.

A versioning convention should be adopted. It is usually best to follow the widely adopted [semantic versioning](https://semver.org/) MAJOR.MINOR.PATCH convention.

### Last updated

The ```last updated``` field refers to the documentation's publication date. Follow the date naming convention from your project's style guide, such as [Google style guide's date guidance](https://developers.google.com/style/dates-times).

Make sure you use an unambiguous date format. Note that 4/5/1900 could be:
* April 5, 1900 in the United States.
* 4 May, 1900 in England.

If adopting the short hand formatting, select the universal date format: ```YYYY-MM-DD``` or ```YYYY-MM```.

### Application version(s)
Where applicable, the documentation should list the version, or range of versions, of the application(s) this documentation describes.

### {Other metadata field}

{Tips for using this field}

### Indicative reading time

Reading speed usually should not be included in fields. There are two lines of thought around including a ```reading time``` field.

Pros:
* It helps someone decide whether they have time to read the page.

Cons:
* It is hard to account for:
    * The range of technial expertise and reading speeds of readers.
    * The varying technical complexity of source material.
    * Multiple authors applying differing rules to assess reading time.
* It potentially makes slow readers feel inadequate and demotivated.
* Reading time is less appicable for some doctypes.

Guidelines for calculating reading time:
* Base estimates on the least experienced and slowest target reader.
* Typically assume a reading speed of 50 words per minute for technical material, and 200 words per typical business material. [ExecuRead reading speed source assessment](https://secure.execuread.com/facts/#:~:text=The%20average%20reading%20speed%20is,roughly%202%20minutes%20per%20page.).

_TBD: Provide better researched references and theory to this._


### Optional: Machine readable metadata

Ideally include machine readable metadata to help search engine optimazation. This should be written in [JSON-LD](http://json-ld.org/) format, such as:

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

The metadata fields which should be presented by a document depends upon:
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

## {Sections and subsections}

* Include standard headings applicable for this template’s `doctype`.
* Where applicable, provide standard text for relevant sections.
* Include tips for doc authors.
* Some sections will be optional and so should include the "optional" tip to the doc author.

## What’s next

This section is optional.


{Template author tip: Most `doctypes` should provide links to help a document author find related topics and next steps.}

{Tip:

* This section is optional.
* Think about the persona(s) of your reader, and consider what they might want to know next. 
* Provide one to four links to more information. Links should be a logical next step to what has already been read.
    * Don't overwhelm your reader with too many choices. Just select the one link for the most likely next steps.
    * Consider {next steps, similar concepts, background theory}.

}

## Revision history

This section is optional, and typically should not be included.

It is typically only include for formal or impportant documents where readers are likely to be interested in the document's change history. 

It typically should only list major, public facing updates.

## Decision log

This section is optional, and typically should not be included, or should be included in an accompanying document.

It is typically only included for business process documents where readers may challenge the reasoning behind a decision.

## Acknowledgements

* This section is optional.
* Here you can acknowledge source material, and organizations or people who have contributed to this document.