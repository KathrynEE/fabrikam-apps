---
title: Checklist for writing and reviewing Azure DevOps technical content
description: This article lists items to check when contributing or reviewing content contributed to technical content for Azure DevOps 
author: KathrynEE
ms.author: kaelli
manager: douge
ms.prod: non-product-specific
ms.topic: contributor-guide
ms.custom: internal-contributor-guide
ms.date: 10/15/2018
---

# Azure DevOps content review checklist

Contributors and content owners can use this checklist when writing or reviewing content contributed to Azure DevOps repositories. 

Additional resources include: 
- [Writing checklist](writing-principles-checklist.md)
- [Microsoft Cloud Style Guide](https://worldready.cloudapp.net/StyleGuide/Read?id=2696)
- [Term Studio](https://termstudio.azurewebsites.net/Default.aspx)
- [Accessibility guidelines](contribute-accessibility-guidelines.md)

## Structure
- Is the [content appropriate for a technical article](contribute-get-started-channel-guidance.md), as opposed to a blog post or white paper? 
- Introduction makes clear what the article is about 
- Is it clear who the target audience is?
- Is the goal of the article clear? How does it help customers? What problem does it solve?
- Is there any unnecessary content that doesn’t support the intent or help solve the problem?
- Does the article follow [MVC standards for its article type](content-type-comparison.md), is it the right MVC type?  
- Does the flow of the article logical? 
- Does the article file name meet our conventions? Is it located in the right folder? 

## Metadata
- All [required metadata](azure-devops-metadata.md) filled out
- Review metadata for SEO 
- Update the ms.date for new or significantly updated articles
- monikerRange check

## Text
- Review of staged content for any obvious misformatted text
- Header/Platform/Version is provided 
- Headers - no gerunds, Sentence capitalization, short to cause least amount of In this article wrapping 
- Sentence capitalization check – all headers 
- Check all headers - use active verbs in Quickstarts, Tutorials, and How-to Guides
- Use of Prerequisites section where needed
- Modern voice 
	- Are the voice and tone of the text following modern voice guidelines?
	- Is the content concise, conversational, and engaging--but not colloquial?
- Tutorial - contains checklist
- [Fictitious names](https://microsoft.sharepoint.com/sites/LCAWeb/Home/Copyrights-Trademarks-and-Patents/Trademarks/Fictitious-Names-Finder) are used as needed 


## Terms and acronyms
- Check [Term studio](https://termstudio.azurewebsites.net/Default.aspx) as needed around common use terms
- Check suspect terms against the [Microsoft Cloud Style Guide](https://worldready.cloudapp.net/StyleGuide/Read?id=2696)
- Terminology check, are terms correctly used, spelled correctly
- Are technical terms and concepts introduced and explained? 
- Check that acronyms are spelled out on first usage 

## [SEO](contribute-how-to-write-seo-basics.md)
- Does your metadata title, page title (H1), and summary (first paragraph) reflect the words the customer will use when searching for this content, and does it clearly capture the relevance of this topic?  
- Are the expected search keywords and phrases used in the content? 

## Art and images
- See [Screenshots: How to create, format, and embed in documentation](contribute-how-to-create-screenshot.md)
- Review of staged content for any obvious misformatted images
- Check that screenshot size is within height (> 750 pixels) and width (> 725 pixels) limits
- Alt text for screenshots is defined
- Callouts in screenshots use established color and format 
- All screenshots have a gray border
- Screenshots use fictitious names and don't display sensitive information

## Tags: Moniker Tags and Conceptual   
- Have [moniker tags been applied correctly](azure-devops-versioning-monikers.md)? 
- Review staged content for each version to check format and that no moniker labels appear in the text
- Are [Tabbed conceptual tabs](azure-devops-tabbed-conceptual-tags.md) applied correctly using the existing tags defined for Azure DevOps

## Cross linking
- Are there helpful links to related resources?
- Quickstarts and tutorials should contain **Next steps** section
- Do all external links resolve correctly? Do any need update?  
- Are internal links formatted correctly? 
- Should this article be linked to from anywhere else or other product doc sets? 
- Disambiguation – Is there a need to refer the user to some other article to disambiguate terms, for example Work Item Tags versus Git Tags, Azure DevOps Projects and Azure DevOps Project. 

## TOC
- Article has been added to the main [TOC yaml file](toc-management.md)
- Article has been added to secondary TOC yml files where appropriate with shared TOC tagging 
- TOC review - no gerunds
- TOC entry makes sense even if shortened from the article title
- Filtering TOC yields results when using article-specific terms 

 