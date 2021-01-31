# {Doctype} template

{Template author tip:

* This base template captures the structure and common elements that all xxx-templates should follow.
* "Template author tips” should be removed from the final xxx-template.md.
* "Document author tips" and variables in {curly brackets} should remain.
* Adjust other tips to align with the `doctype` you are writing for.

}

{Document author tip:

* This {doctype} template captures the structure and common elements that all {doctype} documents should follow.
* It includes tips (such as this) and variables inside curly brackets. These tips and variables must be replaced or removed from the final document.
* The introduction should concisely explain what this document covers, and the type of person who will be interested in reading the document. It should ideally be limited to two to three short sentences.

}

This document {explains/covers/shows what/how to do something}.

It is designed to help {persona or personas} to achieve/learn {some goal}.

{Document author tip:

* All technical documentation should include [machine readable structured metadata](https://developers.google.com/search/docs/guides/sd-policies) which reflects the content in the page. Structured metadata helps search engines index pages appropriately, and facilitates content reuse. For instance, a page's description and associated image may be included in a search result for the page.
* Within this project we have adopted the [JSON-LD](http://json-ld.org/) format for structured metadata, [as recommended by Google](https://developers.google.com/search/docs/guides/intro-structured-data).
* Metadata fields listed as "must" and "should" for "starter" projects the `doctype-guide-template` table must be included in the metadata below. Other metadata fields should not be included in the `doctype-template`. A docset-owner may add or remove metadata fields when customizing the `doctype-template` for their specific project.
* Refer to the `docset-owner-guide` for deeper discussion about Metadata.
* Note, you will need to view this document as raw markdown in order to see the embedded JSON-LD metadata.

}

<!--Machine readable schema.org structured metadata.-->
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


**This document version:** {This document's version, ideally in [semantic versioning](https://semver.org/) MAJOR.MINOR.PATCH format} 

**Last updated:** {Date in the format of "Month DD, YYYY"}

## {Sections and subsections}

{Template author tip:

* Include standard headings applicable for this template’s `doctype`.
* Where applicable, provide standard text for relevant sections.
* Include tips for doc authors.
* Some sections will be optional and include an "optional" tip to the doc author.
}

{Doc author tip:

* Optionally include this section if {some condition}.

}

## What’s next

{Template author tip: Most `doctypes` should provide links to help a document author find related topics and next steps.}

{Document author tip:

* This section is optional.
* You should include three to five links to more information.
* Links should be a logical next step to what has already been read.
* It will typically include a combination of related documents of this `doctype`, as well as relevant other `doctypes`. For instance, a tutorial may point to the next tutorial in a series, relevant reference material, and background conceptual theory.

}

## Acknowledgements

{Document author tip:

* This section is optional.
* Here you can acknowledge organizations or people who have contributed to this document.

}

This document draws inspiration from:

* [{doctype}-template.md](https://github.com/thegooddocsproject/templates{doctype}), version {1.0.1}.
