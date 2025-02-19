---
title: "Method differences between Azure AD Graph and Microsoft Graph"
description: "Describes method differences between Azure Active Directory (Azure AD) Graph API and Microsoft Graph API (REST)."
author: "FaithOmbongi"
ms.author: ombongifaith
ms.reviewer: dkershaw
ms.localizationpriority: medium
ms.prod: "applications"
ms.date: 11/11/2022
#Customer intent: As a developer, I want to to understand how API methods that differ between Azure AD Graph and Microsoft Graph, so that I can update my code accordingly as I migrate my app from Azure AD Graph to Microsoft Graph.
---

# Method differences between Azure AD Graph and Microsoft Graph

This article is part of *step 1: review API differences* of the [process to migrate apps](migrate-azure-ad-graph-planning-checklist.md).

A handful of Azure Active Directory (Azure AD) Graph methods have changed.  If a method is **not** shown in this list, it's already available in the [v1.0 version](/graph/api/overview) of Microsoft Graph, with exactly the same name as in Azure AD Graph.

|Azure AD Graph <br>(v1.6) method |Microsoft Graph<br>(resource/method)|Comments|
|---|---|---|
| getAvailableExtensionProperties | beta&nbsp;-&nbsp;_Not available_ <br> v1.0&nbsp;-&nbsp;[directoryObjects/getAvailableExtensionProperties](/graph/api/directoryobject-getavailableextensionproperties) |  |
| getObjectsByObjectId | beta&nbsp;-&nbsp;[directoryObjects/getByIds](/graph/api/directoryobject-getbyids?view=graph-rest-beta&preserve-view=true) <br> v1.0&nbsp;-&nbsp;[directoryObjects/getByIds](/graph/api/directoryobject-getbyids) | |
| invalidateAllRefreshTokens | beta&nbsp;-&nbsp;[revokeSignInSessions](/graph/api/user-revokesigninsessions?view=graph-rest-beta&preserve-view=true) <br> v1.0&nbsp;-&nbsp;[revokeSignInSessions](/graph/api/user-revokesigninsessions) | |
| isMemberOf | beta&nbsp;-&nbsp;_Not planned_ <br> v1.0&nbsp;-&nbsp;_Not planned_ | Use [checkMemberGroups](/graph/api/user-checkmembergroups) instead. |
| restore | beta&nbsp;-&nbsp;[restore&nbsp;(applications,&nbsp;users,&nbsp;and&nbsp;groups)](/graph/api/directory-deleteditems-restore?view=graph-rest-beta&preserve-view=true)<br> v1.0&nbsp;-&nbsp;[restore&nbsp;(applications,&nbsp;users,&nbsp;and&nbsp;groups)](/graph/api/directory-deleteditems-restore) | You can also view deleted applications, users, and groups and permanently delete them. |

## Next step

> [!div class="nextstepaction"]
> [Review the migration checklist again](migrate-azure-ad-graph-planning-checklist.md)
