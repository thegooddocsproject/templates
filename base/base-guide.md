# {Doctype} guide

This {doctype}-guide describes the process an author should follow when creating a {doctype} document.

**Version:** {This document's version, in MAJOR.MINOR.PATCH format}

**Last updated:** {Date in the format: *Month DD, _YYYY* or *Month, YYYY*}

## Prerequisites

To make the best use of this guide, it helps if you have a working knowledge of:

* The project's documentation style guide.
* Technical writing basics.

{Tip:

* Refer to the short [highlights from Google’s developer documentation style guide](https://developers.google.com/style/highlights) to quickly learn the essentials.
* If you want more, [Google’s tech writer training](https://developers.google.com/tech-writing) material is freely available.
}

## Front matter

Front matter is the metadata stored at the top of each document.

{Tip:

* All technical documentation should include [machine readable structured metadata](https://developers.google.com/search/docs/guides/sd-policies) which reflects the content in the page. Structured metadata helps search engines index pages appropriately, and facilitates content reuse. For instance, a page's description and associated image may be included in a search result for the page.
* Within this project we have adopted the [JSON-LD](http://json-ld.org/) format for structured metadata, [as recommended by Google](https://developers.google.com/search/docs/guides/intro-structured-data).
* Metadata fields listed as "must" and "should" for "starter" projects the `doctype-guide-template` table must be included in the schema.org metadata below. Other metadata fields should not be included in the `doctype-template`. A docset-owner may add or remove metadata fields when customizing the `doctype-template` for their specific project.
* Refer to the `main-doctype-author-guide` for a deeper discussion about metadata.

}

## Machine readable matadata

TBD: Talk about value of metadata. 

```javascript
<!--Machine readable schema.org structured metadata about this document.-->
<script type="application/ld+json">
{
  "name": "{Title of the document}",
  "description": "{Copy of the summary text}",
  "version": "{This document's version, ideally in MAJOR.MINOR.PATCH format}"
  "datePublished": "{Date in the format of YYYY-MM-DD or YYYY-MM}",
  "license": "{URL to license}",
  "audience": "{persona you are writing for, such as: developer, business manager, …}"
}
</script>
```