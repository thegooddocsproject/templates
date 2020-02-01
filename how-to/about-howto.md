# The How-to Article

### When Do I Need a How-to Article?

Sometimes you need to explain in detail how to do a specific task to a user.
You don't need to teach them concepts, but you do need to prescribe a set of sequential steps they must do in that order otherwise they won't be able to use a feature properly.

This is the job of a How-to article.

How-to articles take the reader through a series of steps required to solve a specific, real-world problem.
Think of them as recipes for getting stuff done!

How-to articles can often be confused with tutorials, but you won't fall into this trap if you remember they are _problem_-oriented not _learning_-oriented.

New users typically don't look for how-to articles when they first start using an application.
How-to articles are used by those who have experience with the product and need a specific question answered.

## Content of Your How-to Article

### About the "Overview" Section

Summarise what the reader will get from reading the how-to articles.

Creating a good overview comes down to thinking about who is going to be using it:

* Are you writing only for end-users? For developers?
* Are you writing only for people who have a certain problem to solve?
* Is it intended for a particular industry.

### About the "Before you Start" section

Have you ever got half-way through a how-to, only to discover you need to go and read other documentation before you can continue?
This section is designed to prevent this from happening in the first place.

Describe what the audience needs to know, or needs to have, before attempting this how-to.
By stating the requirements up-front, you prevent your audience from having a bad experience with your tutorial.

Here are some example Before you Start statements:

```
Make sure you meet the following prerequisites before following the steps:

* API credentials for the {company} v3.5 API.
* Access to the Postman application.
* An understanding about what a RESTful API is conceptually.
* (Optional) A development tool (IDE) that displays API responses formatted for readability.

```

### About the "Step by step guide" sections

When you are explaining steps in a process, it can often be useful to include a screenshot for each part of the process.
What can often happen is that when you try to insert a graphic or screenshot into the flow of the procedure, it breaks the procedural content up and makes the instructions difficult to read.

In the `template-howto.adoc` file, you'll notice the tabular step format in the Step-by-step section of the template.
The tabular format allows you to add in your procedural steps right next to the screenshot and reference steps with call-outs.

If you procedural steps do not require screenshots, then you can default to an ordered list.
You can also get this structure in Markdown, but you may need to resort to HTML tables. For Markdown, keep the list as an Ordered list.

## How-to Article Examples

* **Example 1**.

* **Example 2**.
