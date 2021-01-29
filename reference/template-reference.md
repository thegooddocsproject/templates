---
title: template for reference # Describe the title of your article by replacing "template for reference" with the page name you want to publish.
author: The Good Docs Project
uri-repo: https://github.com/projectname
company: REPLACEME
product: # Set the product parameter to add the product name here. 
app: # Insert the name of the app here.
tags: # Set other global keywords here like app name and product name or any other likely labels. These are comma-separated tags.
---

# Overview
Summarise what this reference article is about. What you put here is reused in the Overview section and include in HTML description tags.

<!--
Begin your Reference topic in this section. 
For help with writing and structuring a reference article, see the README.md in the template directory for basic guidelines and links.
Check out https://www.markdownguide.org/basic-syntax/ if you get stuck with AsciiDoc syntax.
-->

# Parameters
Table 1. Example parameter reference template

|Name |Type |Required |Description |
|:--- |:--- |:--- |:--- |
|productCode|`string`|Yes|Code of the document product to return the schema for. <br> <ul><li>Here is a bulleted list with a \| (pipe) inside a table.</li><li>Another bulleted list.<ul><li>An indented list</li></ul></li><li>Back to the list.</li></ul> |
|||||

# Field reference

![Field reference](https://docs.oracle.com/cloud/latest/marketingcs_gs/OMCAA/Resources/Images/Forms/kbf2.x1.jpg)

Table 2. Example field name reference template

|Name |Type |Required |Description |
|:--- |:--- |:--- |:--- |
|Company|`string`|No|The name of the company the person works at or is representing.|
|First Name|`string`|Yes|The first name of the person requiring training.|
|Last Name|`string`|Yes|The surname of the person requiring training.|

Table 3. Example nested table

<table>
  <tr>
    <th>Col 1</th>
    <th>Col 2</th>
  </tr>
  <tr>   
    <th>Cell 1.1</th>
    <th>Cell 1.2</th>
  </tr>
  <tr>
    <th>Cell 2.1</th>
    <th>Cell 2.2
        <table>
            <tr>
              <th>Nested header 1</th>
              <th>Nested header 2</th>
            </tr>
            <tr>   
              <th>Nested cell 1</th>
              <th>Nested cell 2</th>
            </tr>  
        </table>
    </th>
  </tr>
  <tr>
     <th>Cell 3.1</th>
     <td>Cell 3.2</td>     
  </tr>
</table>