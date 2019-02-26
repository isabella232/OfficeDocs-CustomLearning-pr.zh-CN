---
author: pkrebs
ms.author: pkrebs
title: 概述
ms.date: 02/18/2019
description: 面向管理员的 Office 365 自定义学习概述
ms.openlocfilehash: 98187038b66252523c74d88dd9bfd0f217591bc5
ms.sourcegitcommit: e10085e60ca3f38029fde229fb093e6bc4a34203
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/25/2019
ms.locfileid: "30087531"
---
# <a name="customize-the-learning-experience"></a><span data-ttu-id="b94a7-103">自定义学习体验</span><span class="sxs-lookup"><span data-stu-id="b94a7-103">Customize the Learning Experience</span></span>

<span data-ttu-id="b94a7-p101">引入了适用于 office 365 的自定义学习, Microsoft 提供了旨在加快组织内的 office 365 的使用和采用的新解决方案。使用自定义学习, 可以执行以下操作:</span><span class="sxs-lookup"><span data-stu-id="b94a7-p101">Introducing Custom Learning for Office 365, a new solution from Microsoft designed to speed the usage and adoption of Office 365 within an organization. With Custom Learning, you can:</span></span>
- <span data-ttu-id="b94a7-106">为您的环境定制 Office 365 学习和采用内容</span><span class="sxs-lookup"><span data-stu-id="b94a7-106">Tailor Office 365 learning and adoption content for your environment</span></span> 
- <span data-ttu-id="b94a7-107">隐藏或显示内容以反映组织中支持的服务或功能</span><span class="sxs-lookup"><span data-stu-id="b94a7-107">Hide or show content to reflect the services or features supported in your organization</span></span> 
- <span data-ttu-id="b94a7-108">使用 Microsoft 提供最新的学习内容, 让你的内容和用户保持最新的订阅源</span><span class="sxs-lookup"><span data-stu-id="b94a7-108">Keep your content and users current with an up-to-date feed of learning content from Microsoft</span></span> 
- <span data-ttu-id="b94a7-109">专门针对用户需求构建自定义的播放列表和类别</span><span class="sxs-lookup"><span data-stu-id="b94a7-109">Build custom playlists and categories crafted specifically for your user's needs</span></span>

![cg-introducing](media/cg-introducing.png)

## <a name="how-does-custom-learning-work"></a><span data-ttu-id="b94a7-111">自定义学习的工作原理是什么？</span><span class="sxs-lookup"><span data-stu-id="b94a7-111">How does Custom Learning work?</span></span>

<span data-ttu-id="b94a7-112">适用于 Office 365 的自定义学习 (简短的自定义学习) 包括三个部分:</span><span class="sxs-lookup"><span data-stu-id="b94a7-112">Custom Learning for Office 365 (Custom Learning for short) consists of three parts:</span></span> 
1. <span data-ttu-id="b94a7-113">Microsoft online 目录中的内容的实时订阅源</span><span class="sxs-lookup"><span data-stu-id="b94a7-113">a live feed of content from a Microsoft online catalog</span></span>
2. <span data-ttu-id="b94a7-114">SharePoint 通信网站</span><span class="sxs-lookup"><span data-stu-id="b94a7-114">a SharePoint communication site</span></span>
3. <span data-ttu-id="b94a7-115">SharePoint web 部件</span><span class="sxs-lookup"><span data-stu-id="b94a7-115">a SharePoint web part</span></span> 

![cg-howitworks](media/cg-howitworks.png)

## <a name="requirements-and-permissions"></a><span data-ttu-id="b94a7-117">要求和权限</span><span class="sxs-lookup"><span data-stu-id="b94a7-117">Requirements and Permissions</span></span>

<span data-ttu-id="b94a7-p102">在开始使用本指南之前, 请确保已由 SharePoint 租户管理员设置了自定义学习。如果你不确定是否已设置, 请联系你的 SharePoint 租户管理员以验证是否已安装自定义学习。此外, 请务必获取自定义学习 SharePoint 网站的 URL。如果你是租户管理员且尚未安装自定义学习, 请参阅自定义学习 for Office 365 安装指南。</span><span class="sxs-lookup"><span data-stu-id="b94a7-p102">Before getting started with this guide, ensure that Custom Learning has been set up by your  SharePoint tenant administrator. If you’re not sure if it's been set up, contact your SharePoint tenant administrator to verify that Custom Learning has been installed. Also be sure to get the URL of the Custom Learning SharePoint site. If you are the Tenant Administrator and Custom Learning has not been installed, see the Custom Learning for Office 365 Installation Guide.</span></span> 

### <a name="permissions-to-install-custom-learning"></a><span data-ttu-id="b94a7-122">安装自定义学习的权限</span><span class="sxs-lookup"><span data-stu-id="b94a7-122">Permissions to install Custom Learning</span></span>

- <span data-ttu-id="b94a7-123">Office 365 全局管理员</span><span class="sxs-lookup"><span data-stu-id="b94a7-123">Office 365 Global Administrator</span></span>
- <span data-ttu-id="b94a7-124">SharePoint 管理员</span><span class="sxs-lookup"><span data-stu-id="b94a7-124">SharePoint Administrator</span></span>

### <a name="permissions-to-use-custom-learning-administration-features"></a><span data-ttu-id="b94a7-125">使用自定义学习管理功能的权限</span><span class="sxs-lookup"><span data-stu-id="b94a7-125">Permissions to use Custom Learning Administration features</span></span>

- <span data-ttu-id="b94a7-126">Office 365 SharePoint 管理员/SharePoint 网站所有者权限</span><span class="sxs-lookup"><span data-stu-id="b94a7-126">Office 365 SharePoint Administrator/SharePoint Site Owner Permissions</span></span>
- <span data-ttu-id="b94a7-127">sharepoint 网站集管理员/SharePoint 网站所有者权限</span><span class="sxs-lookup"><span data-stu-id="b94a7-127">SharePoint Site Collection Administrator/SharePoint Site Owner Permissions</span></span>

### <a name="permissions-to-use-the-custom-learning-site-as-a-user"></a><span data-ttu-id="b94a7-128">以用户的形式使用自定义学习网站的权限</span><span class="sxs-lookup"><span data-stu-id="b94a7-128">Permissions to use the Custom Learning site as a user</span></span>

- <span data-ttu-id="b94a7-129">Office 365 用户权限/SharePoint 网站访问者权限或更高权限</span><span class="sxs-lookup"><span data-stu-id="b94a7-129">Office 365 user permissions/SharePoint Site Visitor Permissions or higher</span></span>


