# How-to guide

information_source: Read this document before you start working on the [how-to template](how-to-template.md).

## Introduction

How-to guide takes your users through a series of steps required to solve a specific problem. It shows your users how to solve a real-world problem or complete a task in your application, like how to create an issue in GitHub.

The how-to guide clearly describes a set of ordered sequential steps your users must complete to accomplish a task. The how-to guide assumes that a user has basic knowledge of the application and has already read the quickstart and the tutorial.

Do not use how-to guides to teach concepts.

How-to guides are often confused with tutorials. How-to guides are task-oriented, while tutorials are learning-oriented. The table below identifies the differences between the two.

| Tutorials                                                                                                                                       | How-to                                                                                                   |
| ----------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------- |
| Learning oriented                                                                                                                               | Task oriented                                                                                            |
| Helps beginners or expert users learn a new feature and provide a successful learning experience.                                               | Helps an expert user accomplish a task or troubleshoot an issue.                                         |
| Follows a carefully managed path, from the start to the end.                                                                                    | Aims for a successful result, and guides the user along the safest, surest way to the goal.              |
| Eliminates any unexpected scenarios and provides users with a successful finish.                                                                | Alerts the user to the possibility of unexpected scenarios and provides guidance on how to deal with it. |
| Assumes that users do not have any practical knowledge and must explicitly state any tools, file configurations, conceptual details, and so on. | Assumes that users have the practical knowledge of tools, file configurations, applications, and so on.  |

## Why do I need a how-to?

A how-to guide is often used to help competent users perform a task correctly. It can:

- Demonstrate to your users the different capabilities of your application
- Guide your users to solve a real-world problem within the application through an ordered series of steps.
- Help answer specific questions that users may have
- Make users comfortable using the application.
- Improve the user experience, and help reduce costs by lowering the number of support requests.

New users who want to solve a problem instantly can also benefit, provided the how-to is well-written and states any prerequisite knowledge required to complete the task.

## Before Writing A how-to

Before you start working on your how-to, identify:

- The main use cases of your application.
- The different scenarios that your user may encounter in the real world while completing a task. or example, multiple ways through which a task can be completed. If this, then that. In the case of …, an alternative approach is to…
- The surest and the safest way to complete a task. By suggesting multiple ways to complete a task, you're asking users to think through the different ways and choose. Save your users' time and effort by eliminating the options.
- The different error scenarios that a user may encounter while completing a task. and the solutions for the same.

## Best Practices For Writing A how-to

1. Prepare your users for the unexpected, alert the user to its possibility and provide guidance on how to deal with it. For example, include callouts such as warnings, caution, or note to communicate important information while completing a task.
2. Use conditional imperatives. If you want x, do y. To achieve w, do z.
3. Do not explain concepts.
4. Do not provide too many links within the guide. Keep your users on a single page as much as possible. Instead, provide links to additional resources at the bottom of the page.
5. Avoid writing guides for edge cases at the outer boundaries of your application’s capability.
6. Test your how-to guide instructions from start to finish so that you can uncover omitted steps, incorrect details, steps out of order, and information gaps that block users.

## About the "Overview" section

Use this section to provide the following:

- A clear description of the problem or the task that the user can solve or complete.
- When and why your user might want to perform the task. For example, in a guide for creating a pull request, you might tell users that pull requests are used to let others know about the changes you have pushed to a branch on a repository.

Note: The how-to guide assumes that a user has basic knowledge of the application and knows what they want to achieve.

If there are multiple scenarios under which the task can be completed, then create a table as shown below and hyperlink the different how-to guides available for each scenario.

| Guide                             | Scenario                                             |
| --------------------------------- | ---------------------------------------------------- |
| Create a pull request from a fork | The user does not have write permission to the repo. |
| Create a pull request             | The user has write permission to the repo.           |

## About the "Before you begin" section

In this section describe what your users need to know, or need to have before they attempt the how-to. By stating the requirements up-front, you prevent your users from getting halfway through and discovering that they need to go and read other documentation before they can continue.

Use this section to communicate any prerequisites for this how-to, such as:

- Familiarity with the application
- Software and tools needed
- Environments to set up and configure
- Authentication and authorization information
- Other guides or information to read
- Links to procedures or information, or any useful pointers about how to get what they need.

For example:

```markdown
Before you begin, make sure you meet these prerequisites:

- API credentials for the v3.5 API. For more information about accessing your API credentials, see http://example.com/access_your_api_credentials.
- Access to the Postman application.
- A conceptual understanding of RESTful APIs. For more information, see http://example.com/restful_apis.
- (Optional) A development environment (IDE) that displays API responses formatted for readability.
- A list of favourites prepared, so you can manage them. For more information about favourites lists, see http://example.com/favorite_lists.
```

For easy understanding, consider classifying the prerequisites into different categories such as software prerequisites, and hardware prerequisites.

Optionally, provide any helpful cues that signal to a user that they’re probably not in the right place and provide them with more suitable options. For example, If you are a Linux user, then refer to {link to relevant Linux how-to guide}.

## About the "Steps" section

The steps section is where you describe what the user needs to do. Use an ordered list structure to document the how-to steps. How you write your steps will vary depending on your organization's style guide. The template organizes the steps in the following way:

{Task name}

1. {Write the action to take here. Start with a verb.}

   {Optional: Explanatory text}

   {Optional: Code sample or screenshot that helps your users complete this step}

   {Optional: Result}

### Tips for writing steps

- For task names, start with a bare infinitive also known as plain form or base form verbs. For example, “connect”, “set up”, or “build” and express the heading as a complete thought. Don't use the -ing form of the verb because it is harder to translate. Instead of saying, "Connect", you might say, "Connect to the VM instance”.
- For each step, optionally provide some background information about the task so users know what they're about to do and why. Continuing with the example, you might provide some best practices for creating memorable repository names.
- Optionally, add a code sample or screenshot after the explanatory text, depending on the type of how-to you're writing. Screenshots are a great way to show specific parts of the screen you are referring to in a step. Make sure your code samples work.
- Remember to orient your users when walking them through each step. If they need to open a particular file or dialogue box to complete the task, provide that information first.
- Provide examples of sample output such as return data, and a message so that the users can validate whether they performed the step correctly or not. Continuing with the example, you might describe what happens after a user clicks the "Create repository" button.
- Use plain language and define the terminology of any technical term next to it.
- Include one action in a step.

Here is an example step:

Create repository

1. Enter a name for your new repository.
   Good repository names are short and self-explanatory. Avoid repository names with three or more words. After you click "Create repository", GitHub creates your repository and the main page for the repository is displayed. If needed, you can add substeps below a primary step. Make sure to indent the substep one tab space over if you're using Markdown.

Create pull request

1. 2. To create a pull request, do the following:

a. Navigate to the main page of your repository.

b. Under your repository name, click **Pull requests**. By default, all open pull requests are displayed.

c. If you're including code samples in your steps, make sure they are also indented correctly:

Set your Git username for your repository. You can change the name that is associated with your Git commits using the git config command. git config user.name "Dakota Everson"

## About the "See also" section

It's likely that during the course of explaining a multi-task process you will touch on other topics related to the current one, but not strictly required. This section is useful to provide your users with suggestions on further reading without interrupting the topic covered by the current document. An example might be setting up an email client, which requires working credentials to an active email address. The reader need not know how to install and run his/her own email server in order to acquire that access, although this is potentially useful. The link to documentation on running a local mail server could therefore be included in the "See also" section.

## Additional resources

[Diataxis framework](https://diataxis.fr/)

[Docs for Developers](https://docsfordevelopers.com/)
