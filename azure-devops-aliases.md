---
title: Email distribution list aliases for Azure DevOps technical content
description: This article lists email distribution list aliases for technical content for Azure DevOps contributors
author: KathrynEE
ms.author: kaelli
manager: douge
ms.prod: non-product-specific
ms.topic: contributor-guide
ms.custom: internal-contributor-guide
ms.date: 10/15/2018
---

# Aliases for Azure DevOps technical content

Azure DevOps contributors to technical documentation need to belong to certain aliases and be aware of others for information sharing. 

| Alias name | Alias | Required? | Purpose |
| :----------|:------|:----------|:--------|
| APEX Azure DevOps Content Devs | AzDevContentDev | For FTE content developers | FTE communications for content developers (CPub discipline) who oversee major content areas and docsets for Azure DevOps| 
| Azure DevOps | azuredevops | | Email notifications about Azure DevOps | 


## Azure DevOps vsts-docs-pr repo and branch policies

The following groups are added to the Branch Policies for one or more folders in the **vsts-docs-pr** repository. By joining a group, you'll be able to approve your PRs so that they are merged into the master branch. You join these groups by going to [IDWEB](https://idweb/IdentityManagement/default.aspx). 


| Security Group | Web ID Alias | Owner | Purpose |  
| :----------|:------|:--------|:--------|    
| Azure Boards Content Approvers |ts-work-cnt-approve | kaelli | For content contributors to **Azure Boards** and the **/boards**, **/organizations/settings/work** and **/reference** folders |
| Azure DevOps Artifacts Approvers  |az-artifacts-approve | elbatk | For content contributors to the **/artifacts** folder |
| Azure DevOps Collaborate Content Approvers  |ts-collbrt-cnt-appro |kaelli | For content contributors to the **/project** and **/notifications** folders |
| Azure DevOps Release Notes |AzDevRelNotesApprove | alexn|For content contributors to the **/release-notes** folder |
| Azure DevOps Report Content Approvers |ts-repor-cnt-approve | kaelli | For content contributors to the **/report** folder and Analytics content  |
| Azure DevOps Setup-admin Approvers |vsts-setup-approvers | kaelli | For content contributors to the **/organizations** folder |
| Team Services CI/CD Content Approvers | ts-cicd-doc-approve | alewis | For all contributors to **Azure Pipelines** content and the **/pipelines** and **/deploy-azure** folders | 
| Team Services Integrate Approvers | ts-integrate-approve | elbatk | For all contributors to content to the following folders **/integrate**, **/extend**, **/service-hooks**, and **/marketplace** | 
| Team Services Article Approvers | ts-articles-approve | douge | For content contributors to the **/articles** folder | 
| [TechnicalContent]/Azure DevOps Test Content Approvers | N/A | ahomer | For content contributors to the **/test** folder | 
| VSTS VC Doc Approvers |vsts-vc-docapprovers |sdanie | For content contributors to the **/repos** folder | 

These folders are missing from Branch policies: /demo-gen, /java, 

## Azure DevOps tfs-docs-pr repo and branch policies

The following groups are added to the Branch Policies for one or more folders in the **tfs-docs-pr** repository. By joining a group, you'll be able to approve your PRs so that they are merged into the master branch. 

| Security Group | Web ID Alias | Owner | Purpose |
| :----------|:------|:--------|:--------|  
| Azure DevOps TFS Content Approvers  |tfs-setup-approvers | elbatk |For content contributors to the tfs-docs-pr repository  |


 