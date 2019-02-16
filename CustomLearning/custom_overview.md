---
author: pkrebs
ms.author: pkrebs
title: 概述
ms.date: 02/15/2019
description: 面向管理员的 Office 365 自定义学习概述
ms.openlocfilehash: c4b9679ae5a7158306bfd53e345f8e892ab206bc
ms.sourcegitcommit: afb5502604d271f49f6d1133db9dfc499f710eec
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/15/2019
ms.locfileid: "30064982"
---
# <a name="overview-of-custom-learning"></a><span data-ttu-id="99a20-103">自定义学习概述</span><span class="sxs-lookup"><span data-stu-id="99a20-103">Overview of Custom Learning</span></span>
<span data-ttu-id="99a20-p101">引入了适用于 office 365 的自定义学习, Microsoft 提供了旨在加快组织内的 office 365 的使用和采用的新解决方案。使用自定义学习, 可以执行以下操作:</span><span class="sxs-lookup"><span data-stu-id="99a20-p101">Introducing Custom Learning for Office 365, a new solution from Microsoft designed to speed the usage and adoption of Office 365 within an organization. With Custom Learning, you can:</span></span>

- <span data-ttu-id="99a20-p102">为您的环境定制适用于 Office 365 的自定义学习。使用你的品牌和徽标、培训活动和支持信息修改网站页面。隐藏和显示组织中不支持的服务或功能的内容。</span><span class="sxs-lookup"><span data-stu-id="99a20-p102">Tailor Custom Learning for Office 365 to your environment. Modify site pages with your brand and logo, training events, and support info. Hide and show content for services or features that are not supported in your organization.</span></span> 
- <span data-ttu-id="99a20-109">让 microsoft 让你的内容和用户保持最新-自定义学习提供了 Microsoft 保持最新的学习内容的动态订阅源。</span><span class="sxs-lookup"><span data-stu-id="99a20-109">Let Microsoft keep your content and users up-to-date – Custom Learning provides a dynamic feed of learning content that Microsoft keeps up-to-date.</span></span> 
- <span data-ttu-id="99a20-110">构建类别和自定义播放列表, 以反映组织的策略、过程和区域性, 使用户能够根据自己的需要构建学习内容专门设计的技能。</span><span class="sxs-lookup"><span data-stu-id="99a20-110">Build categories and custom playlists reflecting your organization’s policies, procedures, and culture, enabling users to build skills with learning content crafted specifically to their needs.</span></span>

![cg_introducing](media/cg_introducing.png)

## <a name="how-does-custom-learning-word"></a><span data-ttu-id="99a20-112">自定义学习词如何？</span><span class="sxs-lookup"><span data-stu-id="99a20-112">How does Custom Learning word?</span></span>
<span data-ttu-id="99a20-113">适用于 Office 365 的自定义学习 (简短的自定义学习) 包括三个部分:</span><span class="sxs-lookup"><span data-stu-id="99a20-113">Custom Learning for Office 365 (Custom Learning for short) consists of three parts:</span></span> 
- <span data-ttu-id="99a20-114">SharePoint 通信网站</span><span class="sxs-lookup"><span data-stu-id="99a20-114">a SharePoint communication site</span></span>
- <span data-ttu-id="99a20-115">SharePoint web 部件</span><span class="sxs-lookup"><span data-stu-id="99a20-115">a SharePoint web part</span></span>
- <span data-ttu-id="99a20-116">Microsoft online 目录中的内容的实时订阅源</span><span class="sxs-lookup"><span data-stu-id="99a20-116">a live feed of content from a Microsoft online catalog</span></span>

![cg_howitworks](media/cg_howitworks.png)

## <a name="requirements-and-permissions"></a><span data-ttu-id="99a20-118">要求和权限</span><span class="sxs-lookup"><span data-stu-id="99a20-118">Requirements and Permissions</span></span>
<span data-ttu-id="99a20-p103">Office 365 的自定义学习必须由组织的租户管理员 (拥有租户管理员权限的人员) 安装。在开始使用本指南所述的自定义过程之前, 请确保已由 SharePoint 租户管理员设置了自定义学习。如果不确定, 请与您的 SharePoint 租户管理员联系, 以验证是否已安装自定义学习。此外, 请务必获取自定义学习 SharePoint 网站的 URL。如果你是租户管理员且尚未安装自定义学习, 请参阅自定义学习 for Office 365 安装指南。</span><span class="sxs-lookup"><span data-stu-id="99a20-p103">Custom Learning for Office 365 must be installed by your organization’s tenant administrator - someone who has Tenant Administrator permission. Before getting started with this customization procedures covered in this guide, ensure that Custom Learning has been set up by a SharePoint tenant administrator. If you’re not sure, contact your SharePoint tenant administrator to verify that Custom Learning has been installed. Also be sure to get the URL of the Custom Learning SharePoint site. If you are the Tenant Administrator and Custom Learning has not been installed, see the Custom Learning for Office 365 Installation Guide.</span></span> 

### <a name="permissions-required-for-custom-learning"></a><span data-ttu-id="99a20-124">自定义学习所需的权限</span><span class="sxs-lookup"><span data-stu-id="99a20-124">Permissions required for Custom Learning</span></span> 
<span data-ttu-id="99a20-125">以下是安装、自定义和使用自定义学习所需的权限细目。</span><span class="sxs-lookup"><span data-stu-id="99a20-125">Here’s a breakdown of the permissions required for installing, customizing, and using Custom Learning.</span></span> 

<span data-ttu-id="99a20-126">**安装自定义学习的权限**</span><span class="sxs-lookup"><span data-stu-id="99a20-126">**Permissions to install Custom Learning**</span></span>
- <span data-ttu-id="99a20-127">Office 365 全局管理员</span><span class="sxs-lookup"><span data-stu-id="99a20-127">Office 365 Global Administrator</span></span>
- <span data-ttu-id="99a20-128">SharePoint 管理员</span><span class="sxs-lookup"><span data-stu-id="99a20-128">SharePoint Administrator</span></span>

<span data-ttu-id="99a20-129">**使用自定义学习管理功能的权限**</span><span class="sxs-lookup"><span data-stu-id="99a20-129">**Permissions to use Custom Learning Administration features**</span></span>
- <span data-ttu-id="99a20-130">Office 365 SharePoint 管理员/SharePoint 网站所有者权限</span><span class="sxs-lookup"><span data-stu-id="99a20-130">Office 365 SharePoint Administrator/SharePoint Site Owner Permissions</span></span>
- <span data-ttu-id="99a20-131">sharepoint 网站集管理员/SharePoint 网站所有者权限</span><span class="sxs-lookup"><span data-stu-id="99a20-131">SharePoint Site Collection Administrator/SharePoint Site Owner Permissions</span></span>

<span data-ttu-id="99a20-132">**以用户的形式使用自定义学习网站**</span><span class="sxs-lookup"><span data-stu-id="99a20-132">**To use the Custom Learning site as a user**</span></span>
- <span data-ttu-id="99a20-133">Office 365 用户权限/SharePoint 网站访问者权限或更高权限</span><span class="sxs-lookup"><span data-stu-id="99a20-133">Office 365 user permissions/SharePoint Site Visitor Permissions or higher</span></span>
- <span data-ttu-id="99a20-134">如果你不确定是否已向你授予了必要的权限, 请与你的 SharePoint 租户管理员联系。</span><span class="sxs-lookup"><span data-stu-id="99a20-134">If you’re not sure if you’ve been granted the necessary permissions, contact your SharePoint Tenant Administrator.</span></span>

### <a name="next-steps"></a><span data-ttu-id="99a20-135">后续步骤</span><span class="sxs-lookup"><span data-stu-id="99a20-135">Next Steps</span></span>

- [<span data-ttu-id="99a20-136">自定义和共享播放列表</span><span class="sxs-lookup"><span data-stu-id="99a20-136">Customize and Share Playlists</span></span>](customplaylist.md)
- [<span data-ttu-id="99a20-137">推动采用</span><span class="sxs-lookup"><span data-stu-id="99a20-137">Drive Adoption</span></span>](driveadoption.md) 