---
title: Tabbed conceptual tags usage for Azure DevOps technical content
description: Understand how conceptual tabs are used to display different versions of  technical content for Azure DevOps contributors
author: KathrynEE
ms.author: kaelli
manager: douge
ms.prod: non-product-specific
ms.topic: contributor-guide
ms.custom: internal-contributor-guide
ms.date: 10/15/2018
---

# Azure DevOps tabbed conceptual tags usage and guidance

Tabbed conceptual tags are used to provide different versions of content depending on selections made by the user. That selection might cover: 
- Different features supported by the product, such as **New navigation** and **Previous navigation**
- Git repo versus TFVC repo  
- Browser view versus a client view, such as Visual Studio or Team Explorer Everywhere 
- OS differences 
- New work item form versus old form 

> [!NOTE]  
> Tabbed conceptual tags differ from [versioning moniker tags](/azure-devops-versioning-monikers) which are used to support differences in content among different product versions. 

## Syntax for usage
The syntax for using tabbed conceptual tags is simple, as shown in the following example:  

```
# [New navigation](#tab/new-nav)

<!--- Content here  -->

# [Previous navigation](#tab/previous-nav)

<!--- Content here  -->

--- 

```

The last three dashes close out the tabbed conceptual entry. 

### Examples used in articles 
- Uses **New navigation** and **Previous navigation**: 
	- [Open a service, page, or settings](https://docs.microsoft.comazure/devops/project/navigation/go-to-service-page?view=vsts&tabs=new-nav), [Markdown file](https://dev.azure.com/mseng/TechnicalContent/_git/vsts-docs-pr?_a=contents&path=%2Fdocs%2Fproject%2Fnavigation%2Fgo-to-service-page.md&version=GBmaster)
- Uses **Browser** and **Visual Studio**: 
	- [Use work item templates](https://docs.microsoft.comazure/devops/boards/backlogs/work-item-template), [Markdown file](https://mseng.visualstudio.com/TechnicalContent/_git/vsts-docs-pr?_a=contents&path=%2Fdocs%2Fboards%2Fbacklogs%2Fwork-item-template.md&version=GBmaster)
- Uses **New form**, **Old form**, **Visual Studio**, and **Team Explorer Everywhere**: 
	- [Link work items to support traceability and manage dependencies](https://docs.microsoft.comazure/devops/queries/link-work-items-support-traceability)

## Guidance on using tabbed conceptual tags 
- If you use Tabbed Conceptual tags, you need to use the same set throughout the article. That is, you can't use different sets of tags or two tags in one place and three tags in another place within the same article.

## Guidance on using Tabbed Conceptual tags and Conceptual Versioning Moniker tags
  
- Can use moniker tags within a Tabbed Conceptual tag, but not vice-versa; that is, you can't surround a Tabbed Conceptual set of tags with monikers 

## Tags to use

Here are the tags that are in use. Use these tags whenever possible. Wherever possible, we need to use the same tags everywhere. 
If you have to add new tags, add them to this list. 

| Label	| Tag	 | Notes, article where used  |
|----------|---------|-----| 
| New navigation  |  new-nav  | Used to differentiate UI differences when New navigation is enabled  | 
| Previous navigation  |  previous-nav  |  Used to differentiate UI differences when New navigation is disabled |     
| New web form  |  new-web-form   |   /boards content|
| Old web form  |  old-web-form   |   /boards content|
| Designer |  designer   |  /pipelines/build content   |  
| YAML  |  yaml   |  /pipelines content  |  
| Web  |  web   |  /pipelines/agents content  | 
| Windows  |  windows  |  /pipelines/agents content  
| macOS and Linus  |  unix  |   /pipelines/agents content  |  
| Azure Repos or TFS repo |  vsts  | /pipelines/apps content   |  
| Azure Repos  |  gitvsts  | /pipelines/apps content   |  
| GitHub repo  |  github  |     /pipelines/apps content | 
| Install them during the build  |  apple-install-during-build  |  \pipelines |   
| Preinstall them on a macOS build agent  | apple-preinstall | \pipelines  |      
| Team Explorer Everywhere  |  tee  |   Used in a few /boards content  |  
| Visual Studio  |  visual-studio  |  /boards and /repos content  |  
| Command Line  |  command-line  |  /repos content |
| MSTest  |  mstest  |   /pipelines content  |  
| NUnit  |  nunit  |   /pipelines content   |  
| Batch  |  batch  | /pipelines content   |  
| PowerShell  |  powershell  | /pipelines content   | 
| Shell  |  shell  | /pipelines content   |  
| Browser  |  browser  |  Use to support the web portal UI view   |  
| HTTP | http | /extend content |
| C# (client library) | csharpclient | /extend content |
| C# (generic) | csharpgeneric | /extend content |
| Node.js (generic) |nodejsgeneric| /extend content |
| Legacy URLs |  vsts  | DUPLICATE USAGE -  /artifacts/quickstarts  |  
| New URLs |  azuredevops  | /artifacts/quickstarts  | 


## Tags to not use

| Label	| Tag	 | Notes |
|----------|---------|-----| 
| Web  |  web  |  Use **Browser** tab instead  |  
| Web Portal  |  vsts-tfs-web-portal  | Use **Browser** tab instead  |

