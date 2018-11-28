---
title: Azure DevOps terminology guidance  
description: Understand brand names and terms to use and not use within Azure DevOps technical content
author: KathrynEE
ms.author: kaelli
manager: douge
ms.prod: non-product-specific
ms.topic: contributor-guide
ms.custom: internal-contributor-guide
ms.date: 10/15/2018
---

# Azure DevOps terminology and branding guidance 

This article provides usage examples and guidance for using the brand names and specific terms for Azure DevOps content. 

Our umbrella suite name is **Azure DevOps**. 

1. Prefer use of the service names, that is, 'Azure Pipelines' when talking about the product
2. When talking about the suite of services, prefer 'Azure DevOps' (don't use "suite")
3. Use Azure DevOps Services and Azure DevOps Server to disambiguate between the cloud & on-premise versions. Where possible just use Azure DevOps as the umbrella term.

**No abbreviations** should be used, such as ADS or ADOS. Internally, you can use AzDev. However, don't use AzDev externally or in social media. Azure DevOps or #AzureDevOps are the only permitted terms. DevOps should always be **CamelCase**.

There is no need to prefix with Microsoft for the name (that is, you do not need to say Microsoft Azure Pipelines). There are no trademark symbols required in licenses or console output.

While the focus for Azure Repos is Git version control, it still supports the centralized version control system, Team Foundation Version Control (TFVC). The command line for TFVC will remain `tf`.

## Product/service names and usage 

> [!IMPORTANT]
> For some period of time, we need to address both the **New Navigation** elements and the **Previous Navigation** elements (previous names). So, when adding or editing content, think through the names used in the user interface based on the navigation steps you're documenting. 

| Name | Previous name | Definition | **Sample usage in docs:** | Notes on usage | 
|---|----|----|----|----|----|
| **Azure DevOps** |  | Umbrella name of Microsoft&#39;s DevOps solutions, which include 5 cloud services (collectively called Azure DevOps Services) and an on-premises product (currently called TFS, will become Azure DevOps Server in March 2019. |*To create an Azure DevOps organization with a personal Microsoft account or a work or school account, go to the [Azure DevOps Services](https://visualstudio.microsoft.com/products/visual-studio-team-services-vs) site.*   | Limit usage as follows:<br/>- Azure DevOps organization, Azure DevOps project, Azure DevOps group.<br/>- Procedural steps documenting a user interface that uses Azure DevOps.<br/>- Otherwise, **DO NOT USE in docs until after TFS is rebranded to Azure DevOps Server in March 2019 unless you are documenting a user interface with &quot;Azure DevOps&quot; in the user interface string.**|
| **Azure DevOps Services** | Replaces: Visual Studio Team Services, VSTS, Team Services, Visual Studio ALM, Visual Studio Team Services (VSTS), Visual Studio Online, VSO  | Umbrella suite name for the hosted or cloud offering. |*In this quickstart, you learn how to view your or another person's permissions which have been set in Azure DevOps Services or Team Foundation Server (TFS).* | - Use only to refer to _the collection of 5 services_. When referring to functionality or features of a specific service, use the name of that service. Do not find and replace previous names with Azure DevOps Services; it&#39;s important to identify the correct individual service.<br/>- Use to disambiguate the cloud offering from the on-premises offering.<br/>- Do not shorten or abbreviate (for example, &quot;DevOps Services&quot;, &quot;ADS&quot;, &quot;ADOS&quot;, etc.) <br/>| 
| **Azure DevOps Server** | Team Foundation Server and TFS | Name of the on-premises Azure DevOps product.|  Example 1 – You have documentation that references on prem in general (no specific version). Continue to call on prem &quot;TFS&quot; until March 2019.<br/>- Example 2 – After 9/5, you blog about a new feature on the service that will be in the next on prem version. Say it will be available in Azure DevOps Server.<br/>- Example 3 – You have an error message that is specific to &quot;TFS 2018 and earlier&quot;. Always keep this as &quot;TFS&quot; since we will not rebrand these shipped versions of TFS.  | **We won't be making that change yet in the product or in the docs until we are close to launching Azure DevOps Server 2019.**  <br/>- We will not go back and update TFS 2018 or earlier. TFS branding will remain for all versions from TFS 2013 through TFS 2018 (including TFS 2018.3).<br/>- **For things that reference TFS on prem in general (clients, tools, documentation, blogs, etc.), we should keep them as &quot;TFS&quot; until Azure DevOps Server 2019 ships in March. Until then, the latest on prem is still TFS 2018, so we should call it &quot;TFS&quot;. For references to the next version of on prem, you can use Azure DevOps Server.**| 
| **Azure Pipelines** | Replaces: Build &amp; Release hub, build and release hub, Visual Studio Team Services Build Service, Visual Studio Team Services Build &amp; Deployment Service | Name of the service/page that hosts the CI/CD functionality | *Go to the Azure Pipelines service in the web UI...* |- Always use &quot;Azure Pipelines&quot;; do not shorten to &quot;Pipelines&quot;.<br/>- If you encounter phrasing like &quot;CI/CD with VSTS&quot;, replace with &quot;CI/CD with Azure Pipelines&quot; rather than &quot;CI/CD with Azure DevOps&quot;. The goal is to be Azure DevOps service specific now whenever possible based on the context of the doc. <br/>For more terminology specific to Azure Pipelines, see [Azure Pipelines terms](#pipelines-terms). |  
| **Azure DevOps Project(s)** |  |A specific Azure service released long before the Azure DevOps brand. |*Configure continuous integration (CI) and continuous delivery (CD) for your .NET core or ASP.NET application with Azure DevOps Project.* |First reference: Azure DevOps Project(s)<br/>Subsequent references: DevOps Project(s)<br/>- Always capitalize Project.<br/>- Singular or plural Project depends on context.<br/>- Only use Azure DevOps Project(s) when referring to the named Azure service. Do not capitalize when referring to the concept formerly known as &quot;team project&quot; in VSTS.<br/>- When referring to a single user-created Azure DevOps Projects project, use &quot;project&quot; unqualified by the service name. |  
| **Azure Boards** | Work | Work management for teams with work item visualization such as Kanban boards.  | *To manage your backlog, go to "Boards"...* |  - Always use &quot;Azure Boards&quot;; do not shorten to &quot;Boards&quot;, except when referring to the user interface.<br/>- If you encounter phrasing like &quot;Work item tracking with VSTS&quot;, replace with &quot;Work item tracking with Azure Boards&quot; rather than &quot;Work item tracking with Azure DevOps&quot;. The goal is to be Azure DevOps service specific now whenever possible based on the context of the doc. | 
| **Azure Repos** | Code | Code Repositories for Git and TFVC.  |  |- Always use &quot;Azure Repos&quot;; do not shorten to &quot;Repos&quot;.<br/>- Awareness: If you encounter phrasing like &quot;Get a VSTS Git repo&quot;, replace with &quot;Get a Git repo with Azure Repos&quot; rather than &quot;Get an Azure DevOps Git Repo&quot;. The goal is to be Azure DevOps service specific now whenever possible based on the context of the doc.  | 
| **Azure Test Plans** | Test | Capabilities for manual testing of apps. |  | - Always use &quot;Azure Test Plans&quot;; do not shorten to &quot;Test Plans&quot;.<br/>- The goal is to be Azure DevOps service-specific where possible. |
| **Azure Artifacts**| Package, Package management, Package extension | Package management and distribution. |  | - Always use &quot;Azure Artifacts&quot;; do not shorten to &quot;Artifacts&quot;.<br/>- The goal is to be Azure DevOps service-specific now whenever possible based on the context of the doc. | 
| **Team Foundation Version Control (TFVC)**|   |  |  | - Always capitalize Version Control. Do not use &quot;Team Foundation version control.&quot;| 


<a id="ui-terms"> </a>
## UI element terminology 

The intent of this table is to capture the current state of terminology and plan for the next few Sprints as we transition to the new branding. This is to ensure consistency between design, product, docs, and marketing.

| Term | Previous term | Definition and notes on usage | 
|---|----|----|
| breadcrumb | | Navigation in global header<br/>**Sample usage in docs:**<br/>*Global breadcrumb* or *breadcrumb in the global header* |
| flyout | | A panel that appears in the right to take further inputs or provide additional information about the selected item.<br/>**Sample usage in docs:**<br/>*My Work flyout is available at the upper right of every page, providing quick access to the items you care about, no matter where you are in Azure DevOps services.* | 
| global header | | Header present on every page, shows location context and provides access to global controls.<br/>Includes homepage, breadcrumb, search, my work, marketplace, user profile |  
| homepage | | https://dev.azure.com<br/><br/>- Use lower case &quot;project&quot; to refer to a project in Azure DevOps. Use Azure DevOps Project(s) to refer to the named Azure service.<br/>- Don&#39;t prepend Azure DevOps unless you really need to disambiguate. For example, use &quot;project&quot; rather than &quot;Azure DevOps project&quot; or &quot;Azure DevOps Services project&quot;.<br/>- If you do need to disambiguate, use &quot;Azure DevOps project&quot;. |  
| lists | | Secondary navigation used to search and filter within “pages” |   
|organization | account, VSTS account, Team Services account |A shared space where users can collaborate on projects. See [https://blogs.msdn.microsoft.com/devops/2018/07/19/adopting-the-word-organization/](https://blogs.msdn.microsoft.com/devops/2018/07/19/adopting-the-word-organization/). <br/>**Sample usage in docs:**<br/>*This article is about adding a project to an Azure DevOps organization or a Team Foundation Service project collection. If instead you want to create an Azure DevOps Project, see [Azure DevOps Project](https://docs.microsoft.comazure/devops-project/).*<br/><br/>- Don't prepend Azure DevOps unless you really need to disambiguate. For example, use &quot;organization&quot; rather than &quot;Azure DevOps organization&quot; or &quot;Azure DevOps Services project&quot;.<br/>- If you need to disambiguate, use &quot;Azure DevOps organization&quot;. |
| pages | tabs, hubs, hub groups | Sections below services + anything else below |    
| pivot | tabs | Navigation between two or more content panes and rely on text headers to label the different sections of content. |  
| project | Team Project, VSTS project, Team Services project |A project provides a repository for source code and a place for a group of people to plan, track progress, and collaborate on building software solutions.<br/>**Sample usage in docs:**<br/>*This article is about adding a project to an Azure DevOps organization or a Team Foundation Service project collection. If instead you want to create an Azure DevOps Project, see [Azure DevOps Project](https://docs.microsoft.comazure/devops-project/).*<br/><br/>Since project is such a generic term, make sure that the context is clear. For example, avoid confusion with Visual Studio Project, etc. when needed |  
| project page | | https://dev.azure.com/your-org/your-project | 
| selectors | | Drop down menus provided to select from a favorite, filter a list of options, or browse all options.<br/>**Sample usage in docs:**<br/>*To quickly navigate to a feature or artifact—such as a dashboard, repository, product backlog, Kanban board, build pipeline—you can use breadcrumbs or selectors.* | 
| services	| Verticals, hub groups, products<br/>**Sample usage in docs:**<br/>*Go to the Services page and enable Azure Boards.*  | Top-level services we sell |
| settings | | There are several levels of settings: personal, team, project settings, organization (and possibly enterprise) | 
| sidebar | | Vertical pane that hosts the left navigation menu | 


<a id="pipelines-terms"> </a>
## Pipelines terminology changes

The following table captures some of the changes made in terminology for pipelines, builds, and releases. Terminology of unified pipelines is not addressed.

|Concept | Previous name | Definition | Sample usage in docs| Notes on usage | 
|---|----|----|----|----|----|
| build pipeline | build definition | A process describing how your app should be built and tested | (a) To create a pipeline, go to … (b) When you are done, save the pipeline and queue a build. (c) Add the following snippet of code to your .azure-pipeline.yml file and push the changes to your Git repository. | The concept of build pipeline is more prominent when you use the web designer in order to author it. When using YAML files, you just author and push a YAML file (for example, .azure-pipeline.yml), and users do not think about "creating" a pipeline. Avoid repeatedly calling out _build pipeline_ and just say _pipeline_ when the context is clear. The verb that is used the most with this noun is _create_ or _edit_. | 
| build | build | The result of running a build pipeline once | (a) Queue a build … (b) View the build logs … (c) If the build fails, check if you made any changes to the pipeline (or to the YAML file) … | This term can be used as a verb in a more general context, for example, build your app. When referring to gestures in Azure pipelines, it is typically used as a noun, for example, queue a build. The verbs that are used the most with this noun are _view_ or _queue_. |  
| artifact | artifact | A build publishes zero or more artifacts. | (a) Add a _Publish artifacts_ task to your build pipeline... (b) Your build published an artifact... (c) Download the artifacts in a release... | A build publishes artifacts, a release downloads and consumes them. Common verbs: _publish_, _download_. | 
| job | phase or Job | A collection of tasks that run as one unit on an agent in a build or deployment | (a) Define a job in your pipeline … (b) You can configure dependencies between jobs ... (c) Configure a matrix for your job … (d) Each job in the build … | Earlier, we used the term "Phase" as a definition-time concept, and "Job" as a run time concept. Now, we use the term job to mean both. Common verbs: _define_, _run_. | 
| agent | agent | Software installed on a machine to run build or deployment jobs | (a) Use the Microsoft-hosted agent … (b) Install an agent … | Wherever ambiguous, we used to call this Build and Release agent. We can continue to do so. | 
| self-hosted agents | private agents | Agents that you set up and manage to run build and deployment jobs | (a) You can use self-hosted agents to … | You can drop 'self-hosted' if it is clear from the context. We are moving away from 'Private agent' since sentences such as 'Use a private agent in a public project' are awkward. | 
| Microsoft-hosted agents | hosted agents | Agents that are set up and managed by Microsoft to run customers' build and deployment jobs | (a) The following software is installed on Hosted VS2017 agents … | Microsoft runs four types of Microsoft-hosted agents - Hosted VS2017, Hosted, Hosted Linux, and Hosted Mac. Use Microsoft-hosted agents when referring to any of these agents. Otherwise, refer to the specific type. This change has been made to be consistent with the change to self-hosted agents.  |
| parallel jobs | concurrent pipelines | A unit of licensing in pipelines | (a) Ensure that you have enough concurrent jobs … | We changed the licensing recently from concurrent pipelines to concurrent jobs. | 
| release pipeline | release definition | A process describing how your app should be deployed to multiple stages |  (a) To create a pipeline, go to … (b) When you are done, save the pipeline, and create a release. | The verb that is used the most with this noun is _create_ or _edit_. | 
| release | release | The result of running a release pipeline once (or) A collection of artifacts that are is being deployed. | (a) Create a release … (b) Deploy the release to a stage …  | This term is used as a noun. Common verbs: _create_, _deploy_ |  
| stage | environment | A logical break in the pipeline needed to separate concerns | (a) Add a stage to the release pipeline … (b) Deploy the release to the QA stage | | 
| deployment | deployment | The result of running a release targeting a single stage | (a) Deploy a release to a stage … (b) Check the deployment logs (c) If the deployment fails, redeploy the release ... | We often mix up release and deployment when the context is clear. But, it would be better to keep them straight. | |
| service connection | service endpoint | The credentials used to connect to a service outside of Azure DevOps services | (a) Configure an Azure service connection … (b) Configure a GitHub service connection … | | 


## Docs URLs

While all links to VSTS docs should redirect, update URLs to the new Azure DevOps urls.

## Project/Service URLs

| Old URL | New URL |
| --- | --- |
| {organization}.visualstudio.com/{project}  | dev.azure.com/{organization}/{project} |
| {account}.visualstudio.com/{project} | dev.azure.com/{organization}/{project} |

## Other URLs

| Old URL | New URL | Link text | Notes |
| --- | --- | --- | --- |
| [**https://twitter.com/vsts**](https://twitter.com/AzureDevOps) | https://twitter.com/AzureDevOps | @AzureDevOps |   |
| [**https://azure.microsoft.com/case-studies/**](https://azure.microsoft.com/case-studies/) | [https://azure.microsoft.com/case-studies/](https://azure.microsoft.com/case-studies/) | Azure DevOps Case Studies |    |
| [**http://visualstudio.marketplace.com/vsts**](http://visualstudio.marketplace.com/vsts) | [http://visualstudio.marketplace.com/azuredevops](http://visualstudio.marketplace.com/azuredevops) | Azure DevOps extensions | Marketplace for both cloud and on-prem so ok to use Azure DevOps without qualifier |
| [**https://azure.microsoft.com/support/devops/**](https://azure.microsoft.com/support/devops/) | [https://azure.microsoft.com/support/devops/](https://azure.microsoft.com/support/devops/) | Azure DevOps support | en-us can be replaced with any locale |
| [**https://social.msdn.microsoft.com/Forumshome?forum=TFService**](https://social.msdn.microsoft.com/Forums/home?forum=TFService) | n/a | Visual Studio Team Services | No change! |
| [**https://visualstudio.uservoice.com/forums/330519-team-services**](https://visualstudio.uservoice.com/forums/330519-team-services) | n/a | Visual Studio Team Services | No change! |
| [**https://stackoverflow.com/questions/tagged/vs-team-services**](https://stackoverflow.com/questions/tagged/azure-devops) | https://stackoverflow.com/questions/tagged/azure-devops | [https://stackoverflow.com/questions/tagged/azure-devops](https://stackoverflow.com/questions/tagged/azure-devops)  |   |