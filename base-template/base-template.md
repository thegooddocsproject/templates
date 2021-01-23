{Template author tip:

* This base template captures the structure and common elements that all doctype templates should follow. It provides guidance for template authors to follow when creating a new template.
* "Template author tips” should be removed from the final {doctype}-template.md. Other tips should remain.
* Adjust other tips to align with the doctype you are writing for.

}

{Document author tip:

* This {doctype} template captures the structure and common elements that all {doctype} documents should follow.
* This template includes tips (such as this) and variables inside curly brackets. These tips and variables must be replaced or removed from the final document.

}

{Document author tip:

* All templates should include snippets of [structured data](https://developers.google.com/search/docs/guides/sd-policies) to help search engines and facilitate content reuse. 

}

{Template author tip:

* Refer to about-base-template.md for discussion about selecting appropriate [schema.org](https://schema.org/) fields.

}

    <!-- Machine readable structured data which stores metadata about this -->
    <!-- document. It follows the http://json-ld.org/ standard. -->
    <script type="application/ld+json">
    {
      "name": "{Title of the document}",
      "description": "{Copy of the summary text.}",
      "version": "{1.0.1}"
      "datePublished": "1900-01-01",
      "license": "http://creativecommons.org/licenses/by/4.0/",
      "audience": "{developer, business manager, …}"
    }
    </script>

_{TBD: We should define and maintain a list of standard audiences. Or ideally, reference an existing list.}_

_{TBD: What else should be included in our structured data?}_

{Doc author tip:

* The first paragraph should concisely explain what this document covers, and the type of person who will be interested in reading the document. It should ideally be limited to two to three short sentences.

}

This document {explains/covers/shows what/how to do something}.

It is designed to help {persona or personas} to achieve/learn {some goal}.

{Docset owner tip:

* Decide on metadata to collect at the front of each document, such as below.

}

**Reading time:** {10 minutes}

_{TBD: Is there a schema.org property for this?}_

**This document version:** {1.0.1} 

{Docset owner tip: You should adopt MAJOR.MINOR.PATCH [semantic versioning](https://semver.org/)}

**Version of the referenced software:** {2.0}

{Docset owner tip: If possible, you should encourage use of MAJOR.MINOR.PATCH [semantic versioning](https://semver.org/).}

**Last updated:** {January 1, 1900}

**License:** {[Creative Commons Attribution 4.0 International License](http://creativecommons.org/licenses/by/4.0/)}


## {Sections and subsections}

{Doc author tip:

* Some sections will be optional. This should be stated up front with something like the following:

}

Optionally include this section if {some condition}.

{Template author tip:

* Include standard headings applicable for this template’s doctype.
* Where applicable, provide standard text for relevant sections.
* Include tips for "docset owner” and "doc author”.

}

## What’s next

{Template author tip: Most doctypes should provide links to help the reader find related topics and next steps.}

{Document author tip:

* This section is optional.
* You should include three to five links to more information.
* Links should be a logical next step to what has already been read.
* It will typically include a combination of more of this doctype, as well as relevant other doctypes. For instance, a tutorial may point to the next tutorial in a series, and well as reference docs for material which has just been discussed.

}

## Acknowledgements

{Docset owner / Document author tip:

* This section is optional.
* Here you can acknowledge organizations or people who have contributed to this document.

}

This document draws inspiration from:

* {Doctype} Template, version {1.0.1}.
