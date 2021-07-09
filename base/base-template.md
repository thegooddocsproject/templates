# {Doctype} template

{Tip:

* This `{doctype}-template` captures the structure and common text that should be included in a `{doctype}` document.
* It includes tips (such as this) and variables inside curly brackets. These tips and variables should be replaced or removed from the final document.

}

{Tip:

  Optional: Include machine readable [JSON-LD](http://json-ld.org/) metadata to help search engine optimization.

}

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

{Tip:

* The opening paragraph stands alone, just under the title. It's purpose is to quickly help the reader decide whether they should read any further.
* It should concisely explain what this document covers, and the type of person who will be interested in reading it.
* It should be limited to one to three short sentences.

}

This document {explains/covers/shows what/how to do something}.

It is designed to help {persona or personas} to achieve/learn {some goal}.

**This document version:** {MAJOR.MINOR.PATCH} 

**Last updated:** {"Month DD, _YYYY" or "Month YYYY"}

**Application version:**

* {Application 1} : {MAJOR.MINOR.PATCH}
* {Application 2} : {MAJOR.MINOR.PATCH} (or later)
* ...


## {Sections}

{Tip:

* Optionally include this section if {some condition}.
* {Section specific tip 1.}
* {Section specific tip 2.}

}

### {Subsections}

{Tip:

* Optionally include this section if {some condition}.
* {Subsection specific tip 1.}
* {Subsection specific tip 2.}

}

## What’s next

Refer to:
* {[Some doc title](https://example.com/somedoc.html) for {next steps}.}
* {[Some doc title](https://example.com/somedoc.html) for {similar concepts}.}
* {[Some doc title](https://example.com/somedoc.html) for {background theory}.}

## Revision history

{Tip:
* This section is optional or can be combined with the ```decision log``` section if needed.

}

The following table describes the history of {all/major} decisions and revisions made to this {document} over time. 

This guide uses the Major.Minor.Patch [semantic versioning](https://semver.org/) convention.

Edition  |  Date          |  Lead Author(s)    |  Link to Repository Commit/Tag
-------  |  ----          |  --------------    |  -----------------------------
0.2    |  {YYYY-MM-DD}  |  {Your name here}  |  Customised for this project's needs
0.1    |  {YYYY-MM-DD}  |  {Your name here}  |  Initial [{doctype}-template {version}](https://github.com/thegooddocsproject/templates/tree/main/{doctype}) from The Good Docs Project.


## Decision log

{Tip:
* This section is optional or can be combined with the ```revision history``` section if needed.

}

The following table describes the history of all decisions made to this {document} over time:

Ref  |  Date         |  Description                               |  Agreed to by
---  |  ----         |  -----------                               |  ------------
1    | {YYYY-MM-DD}  |  {Explain the decision that was made here} |  {Name or role}

## Acknowledgements

This document draws inspiration from:

* [The Good Docs Project](https://thegooddocsproject.dev) templates, version {MAJOR.MINOR.PATH}.
* {...}
