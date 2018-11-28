---
title: Azure DevOps metadata guidance
description: Lists the metadata used to support Azure DevOps technical content
author: KathrynEE
ms.author: kaelli
manager: douge
ms.prod: non-product-specific
ms.topic: contributor-guide
ms.custom: internal-contributor-guide
ms.date: 10/15/2018
---


# Azure DevOps metadata guidance 

We invest a lot to create content for users, decision-makers, influencers, and potential customers. 
Metadata multiplies that investment by:
 
- Helping search engines display our content in search results to help our customers   
- Guiding customers to the information they seek, so they can complete tasks done with our services and products
- Enabling us to track and measure how well our content performs and what needs improvement.

Many of the metadata tags are used in SkyEye reports. 

**General guidance provided here:**
- [Metadata overview](metadata-overview.md)
- [Metadata attributes](metadata-attributes.md)
- [Contributors guide - Metadata](contribute-how-to-write-metadata.md)

**Additional resources:** 
- [SkyEye MetaCop](http://skyeyereports.cloudapp.net/metacop), check your metadata  


## Sample Azure DevOps metadata 

All articles should include metadata at the top. You delimit metadata with three dashes (---) as shown in the following example.  

```
---
title: Add built-in charts to a team dashboard  
titleSuffix: Azure DevOps & TFS  
description: Add system-generated charts or query-based charts to a team dashboard for Azure DevOps or Team Foundation Server   
ms.prod: devops 
ms.technology: devops-analytics 
ms.reviewer: greggboe   
manager: douge  
ms.author: kaelli
author: KathrynEE
ms.topic: quickstart
monikerRange: '>= tfs-2013'
ms.date: 09/20/2018 
---
```

**For _shared include file, provide this metadata:**
```
---
ms.topic: include
---
```

## Required tags

| Tag | Usage |  Example | 
|-------|------| ------|
| title  |  SEO focused title, 60 total char max, inc. spaces<br/> The site identifier, Microsoft Docs, is added to the end of each title | Add built-in charts to a team dashboard  |
| description  | SEO focused description, Minimum 115 characters long. Maximum 145 characters, including spaces.<br/> Important keywords in the first 100 characters.   | Add system-generated charts or query-based charts to a team dashboard  |
| ms.prod  |  Enter the value associated with the product  | devops |
| ms.technology  |   Enter a value associated with the content area  | See [**ms.technology**](#tech) list below |  
| ms.topic | Enter a value that represents the article type  | See [**ms.topic**](#topic) list below |  
| manager  | Microsoft alias of Content team manager (ms.manager works as well) |  douge | 
| ms.author  | Microsoft alias of the primary writer of the content area  | alewis  |
| author  | GitHub alias of the primary writer of the content area  | alewis  |
| ms.date  | Date  of first publish or with a significant update or change in content<br/>Follow the date pattern shown in the example |  09/20/2018  | 

See also additional guidance for [titles and description](#title-description).


## Optional tags 

| Tag | Usage |  Example | 
|-------|------|------|
| titleSuffix | Use to specify an additional site identifier associated with your product brand<br/>Product name that will appear in the browser tab, prepended to "Microsoft Docs" | Azure DevOps & TFS, or Azure DevOps Services, or TFS | 
| ms.reviewer |  Enter the alias of the primary PM or Dev who reviews or helps author the content |  greggboe | 
| ms.assetid |  GUID, not required |  B080CEFA-4D94-44B2-99E3-0E3E85616D04  | 
|ROBOTS| Crawl instruction for the page for web crawlers, default value is “INDEX, FOLLOW”. Other possible values:"INDEX, FOLLOW";"NOINDEX, NOFOLLOW"; "INDEX, NOFOLLOW", "NOINDEX, FOLLOW”.|
|ms.custom |Text field (multiple values are allowed separated by coma).| |
|ms.devlang |List of values can be found here|  | 
|monikerRange | Specifies the versions that apply to the topic. For the home docset, the article wwill appear in the TOC only for the versions specified in the range.  | monikerRange: 'vsts' | 

<a id="tech" > </a>

## ms.technology (for ms.prod: devops) 

| ms.technology	| "Technology" Name strings|  
| ---| ----| 
| devops-analytics | Analytics| 
| devops-accounts |	Accounts | 
| devops-agile |	Agile| 
| devops-artifacts | Artifacts| 
| devops-billing |	Billing| 
| devops-code-git | 	Repos (Git)| 
| devops-code-tfvc |	Repos (TFVC)| 
| devops-collab |	Search and Collaboration, Wiki| 
| devops-cicd	|  Pipelines| 
| devops-ecosystem | Extensibility and Integration | 
| devops-learn | 	Azure DevOps Learn | 
| devops-marketplace |	Marketplace |
| devops-new-user |	New User Guide and Navigation| 
| devops-public-projects | Public Projects (pending) | 
| devops-ref |	VSTS/TFS API Reference| 
| devops-security |	Security and Permissions| 
| devops-settings |	Settings | 
| devops-test |	Test| 
| devops-whitepapers |	DevOps Whitepapers | 
 


<a id="topic" > </a>

## ms.topic values

| ms.topic value | Usage |
|-------|------|
| article | Useful content which is not specific to a product scenario, such as migration or data security. For example,  whitepapers such as Azure DevOps Technical Articles.  | 
|conceptual | Any content linked in a TOC that is NOT marked in metadata as one of the following <br/>- Quickstart<br/>- Tutorial<br/>- Sample<br/>- Reference<br/>- Overview | 
|contributor-guide | Any content authored specifically for inclusion in a  content contributor guide. | 
| include | Use in _shared files that are included in other topics. | 
|interactive-tutorial | Interactive content.  |
|overview | Overview or User Guide articles. Typically live under an **Overview** node in a TOC, or high-level general topic in a New User Guide or Onboarding guide. | 
|quickstart |Any authored content placed under a **Quickstart ** node in a TOC AND that follows the specific guidelines and template for a Quickstart article |
|reference | Any authored (not autogenerated) content placed under a **Reference** node in a TOC. |
| sample |  Any authored (not autogenerated) content placed under a **Samples** or **Examples** node in a TOC. |
| troubleshooting| Any authored content placed under a **Troubleshooting** node in a TOC AND that follows the specific guidelines and template for a Troubleshooting article |
| tutorial | Any authored content placed under a **Tutorials** node in a TOC AND that follows the specific guidelines and template for a Tutorial article |




