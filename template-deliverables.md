# Template deliverables

This document explains the different documentation deliverables that template authors are required to write as part of each template set. First, read our Template Contributing Guide to understand the larger context for these deliverables.

## Table of contents

- [Overview](#overview)
- [Template file](#template-file)
- [Template guide](#template-guide)
- [Deep dive (optional)](#deep-dive-optional)
- [Template example (optional)](#template-example-optional)


## Overview

Each template set should have the following components:

<table>
  <tr>
    <th>Deliverable</th>
    <th>Description and purpose</th>
    <th>Required?</th>
  </tr>
  <tr>
    <td>Template file</td>
    <td>The template file is the raw template for the type of document you are creating. It provides a rough outline of the suggested content and a few embedded writing tips for how to fill in the different sections of the template.</td>
    <td>Required</td>
  </tr>
  <tr>
    <td>Template guide</td>
    <td>This guide provides a deeper explanation of how to fill in the template. It provides a lightweight introduction to the purpose of this documentation and explains how to fill in each section of the document. Any information that is essential to filling out the template should be noted in this guide.</td>
    <td>Required</td>
  </tr>
  <tr>
    <td>Deep dive</td>
    <td>This optional guide is a supplementary guide that can provide additional helpful information to template users such as key research, deeper theories, brainstorming, or pre-writing steps that are too comprehensive or lengthy to be included in the template guide. What is included in this guide may be unique to each template.</td>
    <td>Optional</td>
  </tr>
  <tr>
    <td>Template example</td>
    <td>The Good Docs Project is in the process of designing a fake documentation project that can provide examples of our templates in action. Until this project is ready, it is optional to provide an example of the template. However, if you want to create a fake example as part of your template set, you may do so.</td>
    <td>Optional</td>
  </tr>
</table>

Each template deliverable is explained in the following sections.

## Template file

Example filename: abc-template.md

The template file is the basic template for the type of document you are creating.
It provides a rough outline of the suggested content and a few embedded writing tips for how to fill in the different sections of the template.
The template user will copy this template and begin filling it in or editing it as their starting point in the writing process.

### Content and formatting guidelines

Each template should have this content:
- **The template title** - The type of document this template is for. For example, "Tutorial template" or "README template."" This title should be formatted with the heading 1 weight.
- **Introductory comment** - Include an embedded writing tip at the start that tells users they should first read the accompanying template guide and before-you-start guide before they fill in the template. Put introductory comments in {curly brackets}.
- **The template sections** - Each section of the temple should begin with a heading with the heading 2 weight. The recommended content and some embedded writing tips fall under the headings.
- **Embedded writing tips** - You can provide some lightweight writing tips that provide some tips or hints about what kind of content the template user might choose to put in a section of the document. Put embedded writing tips in {curly brackets}.

> :triangular_flag_on_post: **NOTE: The basic content of the template depends on the type of document you are creating a template for. Different types of documents can have widely varying content needs. While similar document types are likely to require similar structures, other document types may be structured quite differently.**


### Frequently asked questions

**Q: Is it better to include all the possible sections that someone could possibly include in the template file or should it just have the most common sections?**

A: While this is mostly a judgment call on your part as the template author, it might be better to err on the side of being comprehensive.
Don’t forget that in your template guide you can indicate whether it is common or recommended to include this section or not.

**Q: Can I use heading 3 weights for sub-sections?**

A: Yes, but try not to go much deeper than level 3.


## Template guide

Example filename: abc-template-guide.md

This guide provides a deeper explanation of how to fill in the template.
It provides a lightweight introduction to the purpose of this documentation and explains how to fill in each section of the document.

This guide explains the key decisions that the template user needs to make during the writing process.

This guide might also optionally include a checklist of the required components for this type of document.
It might also include a list of helpful resources or examples that were consulted when the template was created.


### Content and formatting guidelines

The template guide should follow the same basic structure:

- **Template guide title** - The type of document this template is for and the words "guide." For example, "Tutorial guide" or "README guide." This title should be formatted with the heading 1 weight.
- **Introductory comment** - Include an embedded writing tip at the start that tells users they should first read this guide and the before-you-start guide before they fill in the template. This comment could also mention how to get the template file. Put introductory comments in {curly brackets}.
- **Why do I need this type of document?** - Provide some of the information about the purpose of this type of document and how it helps your documentation project. The header for this section should be formatted with the heading 2 weight.
- **Content of this template** - This header marks the beginning of the part of the guide that explains how to fill in each section of the guide. It should be formatted with the heading 2 weight.
- **About the {insert section name here} section** - Next, include each section as they appear in the template with the heading 3 weight. For example, if your template includes a "Before you start" section, this heading should say "About the before your start section." And then it should provide guidance about what kind of content goes in that section and why that section might be included in the final document. If the section is optional, indicate why some documents could benefit from that section or why it might be left out. If the template user needs to make a decision about the content in that section, provide guidance about what should go into that section.
- **Checklist (optional)** - If it makes sense to include a checklist of the typical content required for this type of document, include that here.
- **Additional resources (optional)** - If you’d like to point the user to any helpful guides for deeper study or if you want to acknowledge any resources that inspired you while you wrote this template, link to or cite those resources here.
- **Optional sections** - If your template could benefit from these sections, you may add them:
  - User stories
  - Nature of content
  - Priorities for each quality criteria
  - Implementation strategy (e.g. can this doctype be automatically generated from code?)
  - Business case
  - When to include? When not to include?
  - Customization guidelines
  - Maintenance strategy


### Frequently asked questions

Q: No questions yet.


## Deep dive (optional)

Example filename: template-abc-deep-dive.md

This optional guide contains miscellaneous information or guidance that is too comprehensive for the "guide" document. Based on whatever the each unique template needs, this document could include research, deep theories, pre-writing information, and/or any other material that users need to know when implementing this topic. Template writers are encouraged to point/link readers to that document in their guide to encourage users to read it in more depth.

If the template's documentation type has certain key decisions that need to be made with stakeholders or if it has a dependency on some other type of document or process, that should be mentioned in the deep dive guide. Template writers are encouraged to point/link readers to the deep dive document in their template guide to encourage users to read it in more depth.


### Content and formatting guidelines

Each deep dive should have the following sections:

- **Template title deep dive** - The type of document this template is for + "deep dive". For example, "Tutorial deep dive" or "README deep dive." This title should be formatted with the heading 1 weight.
- **Research guidance (optional)** - The rest of this guide should contain guidance for researching or pre-writing this document. For example, if you were writing a tutorial template, you might include guidance about how to select a tutorial project that is meaningful, fun, teaches the concepts you need to cover, and is the right size for the reader. Alternatively, you could provide a list of questions the template user should know the answer to before they start writing.
- **Process or document dependencies (optional)** - Some templates have dependencies on other documents or are dependent on key internal processes that the user needs to create before they can successfully use this template. For example, if the template is for a bug report template, the user needs to think through how their organization will handle bug reports when they receive them.
- **Any additional content that is unique to your template (optional)** - Whatever you consider necessary to provide to your template users to set them up for success, you can include that information here.


### Frequently asked questions

**Q: What if my template is dependent on a type of document that we have a related Good Docs Project template for?**

A: Indicate that dependency in the deep dive document and link to the other template so that users know how to access that template.

**Q: What if my template is dependent on a type of document that we don’t yet have any Good Docs Project templates for?**

A: Create a new issue for that template in the templates repository and indicate that your template is dependent on this content.


## Template example (optional)

Example filename: abc-template-example.md

The Good Docs Project is in the process of designing a fake documentation project that can provide examples of our templates in action. Until this project is ready, it is optional to provide an example of the template.
However, if you want to create a fake example as part of your template set, you may do so.

If you choose not to create a template example, open an issue indicating that this template still needs an example.
