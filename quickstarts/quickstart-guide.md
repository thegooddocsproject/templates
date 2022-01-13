# Quickstart Guide

:information_source: Read this document before you start working on the [quickstart template](template-quickstarts.md)

## Introduction

A quickstart introduces your users to your application for the first time.
It focuses on the **primary feature** of the application and helps your users to start using the application as quickly as possible.

A good quickstart answers the following questions:

- Scope:
  - What is the core purpose of this application?
  - What is the minimal use case which is covered by this quickstart?
- Install (if applicable):
  - How do I download, install, and configure the application?
  - How do I install and configure the application?
  - How can I get any required access keys or authentication credentials?
- Hello  World:
  - How can I run a simple workflow for a core feature or a common use? case.
- Next steps:
  - What other features are available to explore in the application?

A Quickstart guide is often confused with a Getting Started  guide. Though both these documents help the users get acquainted with the application they widely differ in their target audience. 

There are instances where a Marketing guide is often confused with a Quickstart and a Getting Started guide. The inline table gives a brief comparision about the differences. 

| |Quickstart Guide|Getting Started Guide| Marketing Guide|
|--------|----------------|----------------------|---------------|
 |Target Audience|Domain Experts: Know the problem space and are aware of what they need to do|Beginners:New to problem space and the product|Business Decision Maker: Makes strategic decisions on whether to purchase the product 
|Content|Minimal conceptual information|Detailed conceptual information on product/domain| No/less conceptual information. Instead focuses on the benefits and the customers using the product.
|Focus|how-to| how-to and why|  sales

## Why do I need a Quickstart?

A quickstart is often the first opportunity for your user to build an opinion about the technical quality of your project.It can:
- Make users comfortable using the application.
- Work with any application version the user might use.
- Lead to the willingness to handle complex workflows.
- Help the users in exploring additional features.
- Improve customer experience and help to reduce costs by lowering the number of support requests.

## Tips for writing a Quickstart

- Highlight the primary feature of your application.
- Document the quickest/easiest way to implement the primary feature  of your application.
- Pick a use case that the user can complete within 1-2 hours with a preference for a shorter time.
- Do not complicate the quickstart by including error scenarios/complex use cases.
- Lengthy quickstarts can overwhelm users. Consider condensing or removing steps or reevaluating the scope of the quickstart.
- For code samples, ensure that you include:  
	- Any required `import` or `using` statements.
	- Code comments that explain what the code does.

## About the "Metadata" fields

For more information on how to update the metadata, see [Document version](../base/base-guide.md#document-version), [Last Updated](../base/base-guide.md#last-updated), and [Application Version](../base/base-guide.md#application-versions) on the Good Docs Projects Base template.

## About the "Overview" section

Use this section to provide the following:

- A short description of your application and its purpose.
- A description of what the user will accomplish in this quickstart.
- The intended audience for this document. 
- The basic knowledge that you expect the user to have before using this quickstart.

Defining the audience right in the beginning will help the users identify if the quickstart is relevant for them or if they should continue searching.

## About the "Before You Begin" section

Use this section to mention any requirements/configuration prerequisites that the user must complete before they start the quickstart. 
For easy understanding, we recommend that you classify the prerequisites into different categories such as software prerequisites, hardware prerequisites, and so on. 

## About the "Installation" section

Include the installation section :
- If the installation and/or configuration is typically done at the same time, and by the same person running the quickstart.
 
Use this section to provide:
- Basic instructions/commands to install your application.
- Link to the detailed installation guide if applicable.
- Links to the upstream docs for common software installation instructions.

:memo:
- Some quickstarts may not require Installation instructions, in such scenarios, you can use this section to provide steps to tell the users 
how to sign up, obtain user credentials to log in, and any other authorization/authentication-related information.

## About the "Steps" section

The steps section is where you describe what the user needs to do. How you write your steps will vary depending on your organization's style guide.
This template breaks down the quickstart into **parts**. One part of the quickstart may focus on completing several related steps. 
You're welcome to follow this structure or use the step headings on their own. 
If your quickstart involves multiple complex tasks then break it down different logical parts with each part consisting on one or more related steps. For example, 
Part 1 Configure
Step 1.1
Step 1.2
Part 2 Deploy
Step 2.1
Step 2.2
Part 3 Test
Step 3.1
Step 3.2
If your quickstart involves  simple tasks then structure your document with logical step headings (without parts). For example, refer [Google compute engine](https://cloud.google.com/compute/docs/quickstart-windows) 
quickstart.
If your quickstart involves multiple complex tasks such as configuration,testing, deployment then break it down different logical parts as 
Part 1 Configure
Part 2 Deploy
Part 3 Test
 with each part consisting on one or more related steps. 
If your quickstart involves simple and strightforward tasks then structure your document with logical step headings (without parts). For example, refer [Google compute engine](https://cloud.google.com/compute/docs/quickstart-windows) 
quickstart.

**Tips for writing steps in a quickstart**
- Start the heading with a verb and express the step/part headings as a complete thought. For example, you could use the heading **Connect to the VM instance** instead of just **Connect**.   
- For each step, provide some background information about the task so users know what they're about to do and why.
- Remember to orient your users when walking them through each step. If they need to open a particular file or dialog to complete the task, provide that information first.
- Use plain language and define the terminology of any technical term next to it.
- Include just one action in a step.

:memo:
For additional tips on writing steps, see [Writing Procedural Steps](writing-tips.md#writing-procedural-steps) from **The Good Docs Project**.

## About the "Next Steps" section

Use this section to provide links to other tutorials/articles that the users can try after completing the quickstart. 
Consider a logical connect from the current quickstart that can act as a basis for your users’ next learning.  
Optionally you can provide links to relevant resources, like blogs, reference docs, videos, how-tos, and so on under a new heading **See Also**. 

## References

* [What is a quickstart to you?](https://ffeathers.wordpress.com/2018/10/08/what-is-a-quickstart-to-you/) 