# Main docset author guide

This guide explains how to create and customize templates and guides for a specific `doctype`. It includes background reasoning.

The guide is designed to be read by a docset owner, someone responsible for establishing a documentation strategy for a project.

<!--Machine readable schema.org structured metadata about this guide.-->
<script type="application/ld+json">
{
    "name": "Main docset author guide",
    "description": "This guide explains discusses how `doctype` templates and guides for The Good Docs Project can be customized for a specific project's needs.",
    "version": "0.1"
    "datePublished": "2021-02",
    "license": "http://creativecommons.org/licenses/by/4.0/",
    "audience": "project's docset owner"
}
</script>

**Version:** 0.1

**Last updated:** February, 2021

## Prerequisites

To make the best use of this guide, you should have a working knowledge of:

* The project's documentation style guide.
* Technical writing skills.
* [GitHub Flavored Markdown](https://github.github.com/gfm/): The markup language used to write template documentation.
* [Available doctypes templates](https://github.com/thegooddocsproject/templates): To help identify if you need to create a new template or edit an existing one.

## Target audience for template documents

The template documents target multiple audiences:

|**Role**       |**Reads**                                                   |**Creates**  |
|:--------------|:-----------------------------------------------------------|:------------|
|Template author|main-docset-author-guide<br> base-doctype-template<br> base-doctype-guide-template<br> doctype-example-guide|xxx-template<br> xxx-guide-template<br> xxx-example|
|Docset owner   |main-docset-author-guide<br> xxx-templates<br> xxx-guide-templates|xxx-templates<br> xxx-guide-templates|
|Doc author     |xxx-template <br> xxx-guide-template<br> xxx-example        |document     |
|Doc reader     |document                                                    |             |

### Template author

* A template author creates a document set for a specific `doctype`: (xxx-template, xxx-guide-template, and xxx-example).

### Docset owner

A docset owner is responsible for a Documentation Management Plan and [Information Architecture](https://thegooddocsproject.dev/ia-guide.html) for a project. Typical tasks include:

* Select a set of doctype templates for the project.
* Customize xxx-templates and xxx-guide-templates for the project, if required.
* Select a style guide for the project.
* Establish the docset maintenance process.

_{TBD: We should define a template for a Documentation Management Plan, then reference from here.}_

### Document author

A document author writes documents, in line with the xxx-template, xxx-guide-template, and xxx-example. Typically the document author is a subject matter expert and not a dedicated technical writer.

### Document's reader

And of course, we need to understand the needs of the document's target audience.

## Establish a documentation strategy

While templates from The Good Docs Project can be used as is, it is wise to establish a documentation strategy, which is typically coordinated by someone acting in the role of a docset owner.

Responsibilities of a docset owner typically include:

* Select a set of doctype templates for the project.
* Customize templates if needed.
* Select a style guide for the project.
* Integrate templates with the project's documentation platform and toolchain.
* Establish the docset maintenance process.
* Capture documentation decisions within a Documentation Management Plan.

_{TBD: Add link to a Documentation Management Plan Guide.}_

## Inheritance of doctypes

There are common features shared between similar `doctypes`. The following hierarchy shows how doctypes inherit from each other.

Some of these doctypes are considered "abstract", in that they are not considered to be used as a template in themselves, they are just for other `doctypes` to inherit from.

* Base (abstract)
  * Concept (abstract)
    * API Project overview
    * Explanation
  * Task (abstract)
    * API Quickstart
    * How-to
    * Tutorial
  * Reference (abstract)
    * General reference entry
      * API Reference

_{TBD: We don't have Concept, Task and Reference abstract doctypes yet. We might also want to change their names.}_

## Selecting doctypes

When selecting the `doctypes` to include in a project's documentation, consider:
* The nature of the project and communication needs.
* The project's capacity and willingness to maintain the documentation.
* The toolchain you have access to, and any automation that may be available.
* The maturity and quality criteria set for the project.

The following table prioritizes the importance of `doctypes` based on project maturity:

|Template name          |Core type   |Description                                             |Startup|Mature|
|:----------------------|:-----------|:-------------------------------------------------------|:------|:-----|
|API Project overview   |Concept     | An overview of your API                                |Must   |Must  |
|API Quickstart         |Concept,Task| Simplest possible method of implementing your API      |Should |Must  |
|API Reference          |Reference   | List of references related to your API                 |Must   |Must  |
|Explanation            |Concept     | Longer document giving background or context to a topic|Should |Must  |
|How-to                 |Task        | Short series of steps for a particular task            |Should |Must  |
|Tutorial               |Concept,Task| A training document for a product or topic             |Should |Must  |
|General reference entry|Reference   | Specific details about a particular topic              |Must   |Must  |
|Logging reference      |Reference   | Description of log pipelines                           |May    |Should|

**Note:** The terms "Must”, "Should”, and "May” should be interpreted as per [RFC 2119](https://www.ietf.org/rfc/rfc2119.txt).

_{TBD: We should revisit using the Core type column.}_

_{TBD: This is the 0.1 list of templates, we should build upon these.}_

## Metadata

All templates should include metadata, presented in visible form, and also embedded in machine readable [JSON-LD](http://json-ld.org/) format.

The metadata fields which should be presented by a document depends upon:
* The value the metadata field provides to the target audience for the {doctype} doctype.
* The project's capacity to collect and maintain the metadata field. Can it be collected automatically?
* The maturity and quality criteria set for the project.

**Note:** Be careful not to overcommit to the number of metadata fields you introduce into your project's documentation:
* Many metadata fields need to be maintained manually which adds a maintenance burden to the project.
* If any of the metadata on a site is inaccurate or dated, it will reduce the trustworthiness of all content on the site, as the user typically won’t be able to determine which of the content is trustworthy.
* As such, a project should only adopt metadata fields which are automatically maintained by your documentation publishing system, or where there is an established, low-effort process to ensure the metadata is maintained.

Use the following table to help select the metadata fields to include in your {doctype} template:

{Template autor tip:

* Add or remove rows of metadata fields to the following table which are applicable for the `doctype`.

}

|Metadata field    |schema.org name|Typical location in doc         |Priority - startup|Priority - mature|
|:-----------------|:--------------|:-------------------------------|:-----------------|:----------------|
|Title             |name           |\<title> and first \<h1> heading|Must              |Must             |
|Description       |description    |First paragraph summary         |Must              |Must             |
|Doc version       |version        |Front metadata list             |May               |Should           |
|Doc publish date  |datePublished  |Front metadata list             |Must              |Must             |
|Reading time      |-              |Front metadata list             |May               |May              |
|Target app version|-              |Front metadata list or Footer   |May               |Should           |
|License           |license        |Footer                          |Should            |Must             |
|Target audience   |audience       |Within first paragraph summary  |May               |Should           |

**Note:** The terms "Must”, "Should”, and "May” should be interpreted as per [RFC 2119](https://www.ietf.org/rfc/rfc2119.txt).

_(TBD: Discuss/improve recommendations for [schema.org](https://schema.org/) metadata fields. The table above should cover all metadata fields we consider should be recommended in the The Good Docs Project.}_

## Maintenance strategy

The long term health of documentation depends upon the project's ability to establish sustainable maintenance processes for each doctype. If content on a site is inaccurate or dated, it will reduce the trustworthiness of all the content on the site, as the user typically won’t be able to determine which of the content is trustworthy. As such, a project should only create content where there is commitment for continued maintenance of the content.

The strategies selected should be described in your Documentation Management Plan.

_{TBD: We should define a template for a Documentation Management Plan, then reference from here.}_

_{TBD: Describe maintenance strategies, which likely will be grouped by doctypes. The details of these strategies will be worth spinning out into a separate document. Topics to cover:}_
* _Automated documentation generation from code._
* _Automated reports which highlight:_
    * _When documentation is out of date with software._
    * _When documentation hasn’t been reviewed for a while._
* _Integrating documentation checklists into software deployment, build, and test processes._
_}_

