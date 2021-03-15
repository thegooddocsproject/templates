# {reference article title}

## Overview
{Document author tip:
Summarise what this reference article is about. Explain what all the entries defined on the page have in common. What you put here is reused in the Overview section of your doc site and included in HTML description tags. For help with writing and structuring a reference article, see the file about-reference.md in this directory. Check out https://www.markdownguide.org/basic-syntax/ if you need help with markdown syntax.
}

{Document author tip: It can be helpful to split up your reference page into subsets of related enries. For example, the reference page for an API endpoint might include subsets of entries for "General Requirements", "Request Parameters", and "Responses"}. The formats of entries might be different for each subset; for example, "General Requirements" might be a bulleted list, while "Request Parameters" and "Responses" are tables.
}
## {subset of reference entries}

{table or other structured presentation of entries}

{Document author tip: Here is a starter table for a subset of entries for parameters.  

## Parameters

|Name |Type |Required |Description |
|:--- |:--- |:--- |:--- |
|productCode|`string`|Yes|Code of the document product to return the schema for. <br> <ul><li>Here is a bulleted list with a \| (pipe) inside a table.</li><li>Another bulleted list.<ul><li>An indented list</li></ul></li><li>Back to the list.</li></ul> |
|||||

}

{Document author tip: Here is a starter table for a subset of entries for UI form-field references. Each entry refers to an element in the screenshot.

## Form-field References

![Field reference](https://docs.oracle.com/cloud/latest/marketingcs_gs/OMCAA/Resources/Images/Forms/kbf2.x1.jpg)

|Name |Type |Required |Description |
|:--- |:--- |:--- |:--- |
|Company|`string`|No|The name of the company the person works at or is representing.|
|First Name|`string`|Yes|The first name of the person requiring training.|
|Last Name|`string`|Yes|The surname of the person requiring training.|

{Document author tip: Here is example HTML for a nested table.

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

}