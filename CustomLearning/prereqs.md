---
author: karuanag
ms.author: karuanag
title: 安装的先决条件
ms.date: 02/11/2019
description: 自定义学习安装和设置的决策和预备信息
ms.openlocfilehash: 1a57e8fbecfbce4608c8dcb618f4fdc007467789
ms.sourcegitcommit: e10085e60ca3f38029fde229fb093e6bc4a34203
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/25/2019
ms.locfileid: "29989713"
---
# <a name="getting-started"></a><span data-ttu-id="c5d76-103">入门</span><span class="sxs-lookup"><span data-stu-id="c5d76-103">Getting Started</span></span>

<span data-ttu-id="c5d76-p101">适用于 Office 365 的自定义学习将允许你为你的组织提供按需培训解决方案。 在这里, 我们将讨论为成功部署所需执行的先决条件和决策。</span><span class="sxs-lookup"><span data-stu-id="c5d76-p101">Custom Learning for Office 365 will allow you to provide on-demand training solutions for your organization.  Here we will discuss the pre-requisites and decisions you will need to make for a successful deployment.</span></span>

<span data-ttu-id="c5d76-p102">以下说明概述了如何为 Office 365 (CLO365) 设置自定义学习, 包括将 CLO365 通信网站模板和自定义学习 web 部件安装到租户环境中。以下说明介绍了如何通过 SharePoint online 预配服务安装 CLO365, https://provisioning.sharepointpnp.com如果您只想安装在现有 SharePoint Online 通信网站上使用的自定义学习 web 部件, 请参阅[安装自定义 web 部件](installwebpart.md)的说明。</span><span class="sxs-lookup"><span data-stu-id="c5d76-p102">The following instructions outline how to provision Custom Learning for Office 365 (CLO365), including the installation of the CLO365 communication site template and the Custom Learning web part, into your tenant environment. These instructions cover the installation of CLO365 via the SharePoint Online Provisioning Service at https://provisioning.sharepointpnp.com    If you are interested in installing just the Custom Learning web part for use on an existing SharePoint Online communication site, please refer to the instructions for [installing the custom webpart](installwebpart.md).</span></span> 

## <a name="prerequisites"></a><span data-ttu-id="c5d76-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c5d76-108">Prerequisites</span></span>
 
<span data-ttu-id="c5d76-109">若要通过[SharePoint Online 设置服务](https://provisioning.sharepointpnp.com)成功安装 CLO365, 您必须满足以下先决条件:</span><span class="sxs-lookup"><span data-stu-id="c5d76-109">To successfully install CLO365 via the [SharePoint Online Provisioning Service](https://provisioning.sharepointpnp.com) you must meet the following pre-requisites:</span></span> 
 
- <span data-ttu-id="c5d76-110">将设置 CLO365 的个人必须是要安装的目标租户的租户管理员。</span><span class="sxs-lookup"><span data-stu-id="c5d76-110">The individual that will be provisioning CLO365 must be the tenant administrator of the target tenant for install.</span></span>  
- <span data-ttu-id="c5d76-p103">租户的 "应用程序目录" 必须在 SharePoint 管理中心的 "应用程序" 选项中可用。如果您当前没有应用程序目录, 请参阅[SharePoint Online 文档](https://docs.microsoft.com/en-us/sharepoint/use-app-catalog)以设置此功能。</span><span class="sxs-lookup"><span data-stu-id="c5d76-p103">A tenant 'App Catalog' must be available within the 'Apps' option of the SharePoint Admin Center. If you do not have an app catalog currently refer to the [SharePoint Online documentation](https://docs.microsoft.com/en-us/sharepoint/use-app-catalog) to provision this feature.</span></span>  
- <span data-ttu-id="c5d76-p104">将设置 CLO365 的个人必须是目标租户中应用程序目录的网站集所有者才能安装。如果 CLO365 安装程序不是应用程序目录的网站集所有者, 请[完成这些说明](addappadmin.md)并继续。</span><span class="sxs-lookup"><span data-stu-id="c5d76-p104">The individual that will be provisioning CLO365 must be a site collection owner of the app catalog in the target tenant for install. If the CLO365 installer is not a site collection owner of the app catalog [complete these instructions](addappadmin.md) and continue.</span></span>  

### <a name="next-steps---service-decisionsservicedecisionsmd"></a><span data-ttu-id="c5d76-115">后续步骤-[服务决策](servicedecisions.md)</span><span class="sxs-lookup"><span data-stu-id="c5d76-115">Next Steps - [Service Decisions](servicedecisions.md)</span></span>
