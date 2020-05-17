# The reference article

## When do I need a reference article?

Reference articles provides information-oriented descriptions of specific technology parts.

The purpose of reference articles is to tell the facts about the technology as consistently and accurately as possible, without mixing procedural or instructional content.

Reference articles work well when they are:

* consistent in structure, language and tone
* contain descriptive information that is relevant to the reference topic's overview only
* focus on information accuracy and the facts only.

## Content of your reference article

### About the "Overview" section

Summarise what the reader will get from reading the reference article.

Creating a good overview comes down to thinking about who is going to be using it:

* Are you writing only for end-users? For developers?
* Are you writing only for people who have a certain problem to solve?
* Is it intended for a particular industry.

Your overview should be descriptive of the subject you want to cover, so your audience can quickly identify what the reference article is about.

### About the "Body" section

There is no specific structure to use in reference articles because the structure will vary based on the type of factual information you are documenting.

For example, the example included in the more specific `api-reference` template type in this repository describes how you would structure an API endpoint.
This reference structure is prescriptive, but only relevant for this documentation type.

In most cases your content will take on a tabular format of some type.
It is often easier to present reference style information in a table.

Here are some overall suggestions about how you can structure your reference articles.

#### Structure suggestions

Follow these suggestions when structuring and writing your reference topics.

* Employ Don't Repeat Yourself (DRY) methods when writing reference documentation.
** Re-use content using the https://asciidoctor.org/docs/user-manual/#include-directive[Asciidoctor Include Directive] if:
** The content is written for the same audience.
** The content fits in with your reference document without modification.
* If you are referring to a screen in a UI:
** Use a reference table explaining the fields and their meanings.
** Use call-outs in screen shots to help your audience find the field in the reference table.

### Code-generated documentation

Reference articles can often be replaced by _thoroughly-written_ auto-doc output from your code.
This is particularly the case with content such as API reference docs and package descriptions that are documented in code doc-blocks or are produced with tools such as the Open API toolchain.

If you need to provide more narrative style content to complement your API reference endpoints, see the `api-` template types in this repository.

## How-to article examples

* **Example 1**.

* **Example 2**.
