---
title: template for logging
author: The Good Docs Project 
uri-repo: https://github.com/projectname
company: REPLACEME
product: <!-- Set the product parameter to add the product name here. -->
app: <!-- Insert the name of the app here. -->
tags: <!-- Set other global keywords here like app name and product name or any other likely labels. These are comma-separated tags.-->
---

<!--
For help with writing and structuring a log article, see the README.adoc in the template directory for basic guidelines and links.
Check out https://asciidoctor.org/docs/asciidoc-syntax-quick-reference/ if you get stuck with AsciiDoc syntax.
-->
# {pipeline} for {app}

## Description

<table>
  <tr>
    <th>Log pipeline name</th>
    <td>Specify the name of the logstash pipeline in this field.</td>
  </tr>
  <tr>    
    <th>Description</th>
    <td>Summarise why this log format exists, or why you would look for this log. What you put here is reused in the Log description section and included in HTML description tags.</td>
  </tr>
  <tr>
    <th>Log format</th>
    <td>Specify the format of the log file: XML or JSON.</td>
  </tr>
  <tr>
     <th>Log transfer method</th>
     <td>Single-line curl using MSSQL Service Broker. <br>     
     App writes to a log file which is shipped to logstash using filebeat.<br>     
     </td>
  </tr>
  <tr>
     <th>Output location</th>
     <td>If the output location uses curl, then specify a URL similar to https://logs.{company}.com.au/csdb_appflow.<br>         
         If the output location is to a file, specify the `/path/to/the/logfile`.<br>
      </td>
  </tr>  
</table>

## Logging example

Logging example
<!-- source,XML -->
```
<message>
   <detail>
      <dt>2017-05-22T13:35:27.013</dt>
      <appId>4240263</appId>
      <sourceId>3585996</sourceId>
      <refreshId>0</refreshId>
      <dt2>2017-05-22T13:35:27.013+1000</dt2>
      <action>appReady</action>
      <apiGuid>BB31E8B6-88C8-4DEB-9529-8EFD7F680C0B</apiGuid>
   </detail>
</message>
```

## Log properties

In addition to the mandatory logging properties sent for all log pipelines, the following log properties are sent for this pipeline.

| Property name | Description | Logstash type | Logstash type |
| :---        | :----       |:----   |:----   |
| This example row will give you an idea of what to put in this table csdb_appflow.api-guid| The unique API GUID from a <_company_> application flow. This information is extracted from the <apiGuid> element in the XML log| Choose One string integer float |BB31E8B6-88C8-4DEB-9529-8EFD7F680C0B |
