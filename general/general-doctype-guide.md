# General doctype guide

This guide provides common information applicable to most doctype guides. Section headings align with doctype template documents.

It is applicable for for document authors.

It will also help:
* A docset owner select and customize a template set.
* Templateers (template authors) in building a template.

## Prerequisites

To write impactful documentation, it helps if you are familiar with:

* The base-template-set:
    * base-template, base-example, base-guide, base-checklist, base-theory.
* The project's documentation style guide.
    * Refer to the short [highlights from Google’s developer documentation style guide](https://developers.google.com/style/highlights) to quickly learn style essentials.
* Technical writing basics.
    * [Google’s tech writer training](https://developers.google.com/tech-writing) is a good source of material and is freely available.
}

## Common fields

This section discusses the common fields typically included in doctypes.

### Hero description
The hero description is an opening paragraph which stands alone, just under the title. It's purpose is to quickly help the reader decide whether they should read any further.

It should concisely explain what this document covers, and the type of person who will be interested in reading it. It should be limited to one to three short sentences.

### Document version
To enable consistency and traceability between cross-referenced documentation and software, all documentation should be versioned.

A versioning convention should be adopted, preferably the widely adopted [semantic versioning](https://semver.org/) MAJOR.MINOR.PATCH format.

### Last updated

The ```last updated``` field refers to the documentation's publication date. An unambiguous date naming convention should be followed, which should be defined in your project's style guide. For instance, [Google style guide's date guidance](https://developers.google.com/style/dates-times) which recommends long form description of date: ```Month DD, YYYY``` or ```Month, YYYY```.

If adopting the short hand formatting, select the universal date format: ```YYYY-MM-DD``` or ```YYYY-MM```.

Avoid using ```MM/DD/YYYY``` or ```DD/MM/YYYY``` formats as these conventions differ around the world and will confuse readers. 

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

If you do include reading time, apply these guidelines:
* Base estimates on the least experienced and slowest target reader.
* Typically assume a reading speed of 50 words per minute for technical material, and 200 words per typical business material.

  Source: [ExecuRead reading speed source assessment](https://secure.execuread.com/facts/#:~:text=The%20average%20reading%20speed%20is,roughly%202%20minutes%20per%20page.).

_TBD: Provide better researched references and theory to this._

### Application version(s)
The documentation should list the version, or range of versions, of the application(s) this documentation describes.

For example:

```
This guide applies to:
* chronologue-server v1.3
* chronologue-client v5.2 or later
```

### Metadata

All templates should include metadata, presented in visible form. Ideally, your metadata will be embedded in machine readable [JSON-LD](http://json-ld.org/) format too, such as:

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

