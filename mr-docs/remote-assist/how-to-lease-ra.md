---
author: pawinfie
description:  Technical document for deploying cross-tenant or cross-company Remote Assist calls
ms.author: pawinfie
ms.date: 03/24/2020
ms.service: crm-online
ms.topic: article
title: Cross-tenant Remote Assist licensing implementation
ms.reviewer: krbjoran
---

# How to provide Remote Assist licenses to external users

This document assumes that you have read our [Remote Assist External Collaboration Scenarios](out-of-tenant-overview.md) document. 

Information barriers are a great way to control who can search and collaborate with one another when using Microsoft Teams and Remote Assist. Specifically, information barrier policies determine and prevent the following kinds of unauthorized communications:

- Searching for a user
- Adding a member to a team
- Starting a chat session with someone
- Starting a group chat
- Inviting someone to join a meeting
- Sharing a screen
- Placing a call

Additional information about information barriers can be found [here](https://docs.microsoft.com/microsoft-365/compliance/information-barriers?view=o365-worldwide#what-happens-with-information-barriers).

In this article, we'll take a look at how to deploy Remote Assist licenses for users who are outside your tenant. 

## Step 1. Determine if information barriers are necessary

### Overview of information barriers

Information barriers are a great way to control who can search and collaborate with one another when using Microsoft Teams and Remote Assist. Information barriers use Azure Active Directory (Azure AD) attributes to segment Azure AD users. The segmentation of users determines which users can talk to one another.

It's important to plan the segmentation of users. You can segment users based on what department they belong to, what Azure AD group they are a member of, or even by their usage location. A full list of attributes can be found [here](https://docs.microsoft.com/microsoft-365/compliance/information-barriers-attributes?view=o365-worldwide#reference).

### Information barrier example

For example, you may choose to segment users based on the "Group" attribute. You want to allow users in the Azure AD Group "A" to communicate with users in the Azure AD Group "B", but not with the users in Azure AD Group "C". Information barriers can use the "Group" attribute to allow Group A to communicate with Group B but not with Group C.

>[!NOTE]
> To learn more about information barriers, see the following docs:
>
> - [Overview of information barriers](https://docs.microsoft.com/microsoft-365/compliance/information-barriers?view=o365-worldwide).
> - [Overview of segmentation and attributes](https://docs.microsoft.com/microsoft-365/compliance/information-barriers-attributes?view=o365-worldwide).

## Step 2. Buy the correct licenses

The following licenses are required to enable a service account user to use Remote Assist.

- [Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-whatis#who-uses-azure-ad)
- [Remote Assist](buy-remote-assist.md)
- Microsoft Teams

If you would like to control who the service account user can search and collaborate with, you will need to assign the service account a information barrier license. The following licensing suites include information barrier licenses:

- Microsoft 365 E5
- Office 365 E5
- Office 365 Advanced Compliance
- Microsoft 365 E5 Information Protection and Compliance

For more information, see [Updated list of Information Barrier licenses](https://docs.microsoft.com/microsoft-365/compliance/information-barriers?view=o365-worldwide#required-licenses-and-permissions)

>[!NOTE]
> If you are following the steps in the [Deploy HoloLens in a Commercial Environment](https://docs.microsoft.com/hololens/hololens-requirements#apps) article, please go back to that document before implementing this solution.

## Step 3. Create service accounts

Learn how to use Azure AD to [create service accounts](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory) for your external collaborators (e.g., customers and vendors).

## Step 4. Assign licenses

Learn how to [assign licenses](https://docs.microsoft.com/azure/active-directory/fundamentals/license-users-groups) to each service account user. 

## Step 5. Configure information barriers

Finally, you'll need to [configure the information barriers](https://docs.microsoft.com/microsoft-365/compliance/information-barriers-policies?view=o365-worldwide).