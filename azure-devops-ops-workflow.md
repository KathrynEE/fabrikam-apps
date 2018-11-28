---
title: Azure DevOps OPs publishing workflow
description: Describes the workflow used to publish Azure DevOps content
author: KathrynEE
ms.author: kaelli
manager: douge
ms.prod: non-product-specific
ms.topic: contributor-guide
ms.custom: internal-contributor-guide
ms.date: 10/15/2018
---


# Azure DevOps Open Publishing workflow 

Unlike the majority of Microsoft Docs content that is maintained in the MicrosoftDocs GitHub repo, Azure DevOps content is maintained in several Git repos in Azure Repos. For a list of repos, see [Azure DevOps repositories, content areas, content owners](azure-devops-content-areas-and-owners.md).

## Workflow to author and publish content  

> [!TIP]  
> If you are adding new content or making significant changes, please include a member of the content team on this work to avoid duplication and to align with ongoing content strategies. You can find the member of the content team who oversees a specific content area in [Azure DevOps repositories, content areas, content owners](azure-devops-content-areas-and-owners.md). Or email the [Azure DevOps content team](mailto:AzDevContentDev@microsoft.com). 

The current process for authoring and publishing content is:  

1.	Make sure you have permissions to edit and contribute to the TechnicalContent project on [https://azure.dev.com/mseng/TechnicalContent](https://azure.dev.com/mseng/TechnicalContent). You'll need to have been added as a contributor to the project. Most FTEs should have access. 

1.	Clone the [vsts-docs-pr repo](https://dev.azure.com/mseng/TechnicalContent/_git/vsts-docs-pr?version=GBmaster), in Visual Studio or Visual Studio Code.   

1.	Create a new local branch from the **/master** branch. You can do this from Visual Studio or Visual Studio Code. The new working branch will be for your content additions and updates.   

1.	Make your changes to the content and commit them to this working branch.   
	a.	If you are working from a clone repo, push them to the remote repo for your working branch   
	b.	Create a Pull Request from your branch to the master branch.   
	c.	Once you have committed your content to the (remote) repo, a build will kick off. Builds can take 10-15 min, so if you're not sure if you're in the build queue, you can check the [build queue portal](https://ops.microsoft.com/#/repos/00628bb5-0d21-f41a-1556-bbace95a5e89). You will receive an email – probably two emails – that will tell you where the content is staged and if there are broken links – a build report. Link to build report is in the email.  
	d.	Check that your content displays as expected on the staging site.   
	e.	Once your content displays correctly, and there are no build errors, it is ready for review. Add an **@mention** in the PR to the content owner for the folder you are updating for them to review.   
	f.	Upon the content owner's approval, complete the PR.  

1.  Twice a day or more often a PR from master to live is made, at which time your changes will get published. 	


## Contributor's guide resources 
- **Follow content standards**
	- [Write an overview](contribute-how-to-write-overview.md)
	- [Write a quickstart](contribute-how-to-mvc-quickstart.md)
	- [Write a tutorial](contribute-how-to-mvc-tutorial.md)
	- [Write a sample](contribute-how-to-mvc-samples.md)
	- [Edit a TOC](contribute-toc-mvc-how-to.md) 
- **Improve your writing**
	- [Follow writing principles](writing-principles.md)
	- [Review the Microsoft style guide](https://worldready.cloudapp.net/Styleguide/Read?id=2700)  



## Additional notes

### Staged content  
- Any time you push your working branch to the cloud repo, the branch builds. There is no actual build on mseng that you can check,. However, you get email when the build completes along with a link to an error report. There are build definitions you may see on [dev.azure.com/mseng/TechnicalContent](https://dev.azure.com/mseng/TechnicalContent), but they are faux wrapper builds that kick off a build "in the cloud" and just report when the "cloud" build is done. 
- You get staging with a working TOC and links at: 
	```
	https://review.docs.microsoft.comazure/devops/File-path-and-name?branch=branchname 
	```  

	For example: 

	```
	https://review.docs.microsoft.comazure/devops/boards/boards/index?branch=master
	```  
- When you push your branch, you can see where you are in the [OPS Portal](https://ops.microsoft.com/#/repos/00628bb5-0d21-f41a-1556-bbace95a5e89) build queue. You'll receive one or two emails when the build completes for a push or PR.  Dev is working on better build filtering to avoid the two unnecessary builds when you PR. 

- Each area has its own TOC that uses markdown syntax within a yml file (toc.yml), and the TOC on the published site only shows one area's TOC at a time. 
- The UI around navigating across hubs changes to a "breadcrumb" top nav bar where each element in the "breadcrumb" path is a drop-down to other sub nodes at that level.



