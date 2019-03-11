---
author: pkrebs
ms.author: pkrebs
title: 概述
ms.date: 02/18/2019
description: 面向管理员的 Office 365 自定义学习概述
ms.openlocfilehash: 6aee3a93a5109b37e43a7118bd98ca31e8b9ac1f
ms.sourcegitcommit: e0adc8963419a4dd5c4d9bcc9f4f2cc1fbe291d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/10/2019
ms.locfileid: "30523016"
---
# <a name="customize-the-learning-experience"></a><span data-ttu-id="88c01-103">自定义学习体验</span><span class="sxs-lookup"><span data-stu-id="88c01-103">Customize the Learning Experience</span></span>

<span data-ttu-id="88c01-104">引入了适用于 office 365 的自定义学习, Microsoft 提供了旨在加快组织内的 office 365 的使用和采用的新解决方案。</span><span class="sxs-lookup"><span data-stu-id="88c01-104">Introducing Custom Learning for Office 365, a new solution from Microsoft designed to speed the usage and adoption of Office 365 within an organization.</span></span> <span data-ttu-id="88c01-105">使用自定义学习, 可以执行以下操作:</span><span class="sxs-lookup"><span data-stu-id="88c01-105">With Custom Learning, you can:</span></span>
- <span data-ttu-id="88c01-106">为您的环境定制 Office 365 学习和采用内容</span><span class="sxs-lookup"><span data-stu-id="88c01-106">Tailor Office 365 learning and adoption content for your environment</span></span> 
- <span data-ttu-id="88c01-107">隐藏或显示内容以反映组织中支持的服务或功能</span><span class="sxs-lookup"><span data-stu-id="88c01-107">Hide or show content to reflect the services or features supported in your organization</span></span> 
- <span data-ttu-id="88c01-108">使用 Microsoft 提供最新的学习内容, 让你的内容和用户保持最新的订阅源</span><span class="sxs-lookup"><span data-stu-id="88c01-108">Keep your content and users current with an up-to-date feed of learning content from Microsoft</span></span> 
- <span data-ttu-id="88c01-109">专门针对用户需求构建自定义的播放列表和类别</span><span class="sxs-lookup"><span data-stu-id="88c01-109">Build custom playlists and categories crafted specifically for your user's needs</span></span>

![cg-introducing](media/cg-introducing.png)

## <a name="how-does-custom-learning-work"></a><span data-ttu-id="88c01-111">自定义学习的工作原理是什么？</span><span class="sxs-lookup"><span data-stu-id="88c01-111">How does Custom Learning work?</span></span>

<span data-ttu-id="88c01-112">适用于 Office 365 的自定义学习 (简短的自定义学习) 包括三个部分:</span><span class="sxs-lookup"><span data-stu-id="88c01-112">Custom Learning for Office 365 (Custom Learning for short) consists of three parts:</span></span> 
1. <span data-ttu-id="88c01-113">Microsoft online 目录中的内容的实时订阅源</span><span class="sxs-lookup"><span data-stu-id="88c01-113">a live feed of content from a Microsoft online catalog</span></span>
2. <span data-ttu-id="88c01-114">SharePoint 通信网站</span><span class="sxs-lookup"><span data-stu-id="88c01-114">a SharePoint communication site</span></span>
3. <span data-ttu-id="88c01-115">SharePoint web 部件</span><span class="sxs-lookup"><span data-stu-id="88c01-115">a SharePoint web part</span></span> 

![cg-howitworks](media/cg-howitworks.png)

## <a name="requirements-and-permissions"></a><span data-ttu-id="88c01-117">要求和权限</span><span class="sxs-lookup"><span data-stu-id="88c01-117">Requirements and Permissions</span></span>

<span data-ttu-id="88c01-118">在开始使用本指南之前, 请确保已由 SharePoint 租户管理员设置了自定义学习。</span><span class="sxs-lookup"><span data-stu-id="88c01-118">Before getting started with this guide, ensure that Custom Learning has been set up by your SharePoint Tenant Administrator.</span></span> <span data-ttu-id="88c01-119">如果你不确定是否已设置, 请联系你的 SharePoint 租户管理员以验证是否已设置自定义学习。</span><span class="sxs-lookup"><span data-stu-id="88c01-119">If you’re not sure if it's been set up, contact your SharePoint tenant administrator to verify that Custom Learning has been provisioned.</span></span> <span data-ttu-id="88c01-120">此外, 请务必获取自定义学习 SharePoint 网站的 URL。</span><span class="sxs-lookup"><span data-stu-id="88c01-120">Also be sure to get the URL of the Custom Learning SharePoint site.</span></span> <span data-ttu-id="88c01-121">如果你是租户管理员, 且尚未预配自定义学习, 请参阅[设置自定义学习](custom_provision.md)。</span><span class="sxs-lookup"><span data-stu-id="88c01-121">If you are the Tenant Administrator and Custom Learning has not been provisioned, see [Provision Custom Learning](custom_provision.md).</span></span> 

### <a name="permissions-to-provision-custom-learning"></a><span data-ttu-id="88c01-122">设置自定义学习的权限</span><span class="sxs-lookup"><span data-stu-id="88c01-122">Permissions to provision Custom Learning</span></span>

- <span data-ttu-id="88c01-123">租户管理员, 也称为 Office 365 全局管理员</span><span class="sxs-lookup"><span data-stu-id="88c01-123">Tenant Administrator, also known as Office 365 Global Administrator</span></span>
- <span data-ttu-id="88c01-124">具有网站所有者权限的 SharePoint 网站集管理员</span><span class="sxs-lookup"><span data-stu-id="88c01-124">SharePoint Site Collection Administrator with Owner permissions on the site</span></span>

### <a name="permissions-to-use-custom-learning-administration-features"></a><span data-ttu-id="88c01-125">使用自定义学习管理功能的权限</span><span class="sxs-lookup"><span data-stu-id="88c01-125">Permissions to use Custom Learning Administration features</span></span>

- <span data-ttu-id="88c01-126">网站集管理员</span><span class="sxs-lookup"><span data-stu-id="88c01-126">Site Collection Administrator</span></span>
- <span data-ttu-id="88c01-127">SharePoint 所有者或成员权限</span><span class="sxs-lookup"><span data-stu-id="88c01-127">SharePoint Owner or Member permissions</span></span>

### <a name="permissions-to-use-the-custom-learning-site-as-a-user"></a><span data-ttu-id="88c01-128">以用户的形式使用自定义学习网站的权限</span><span class="sxs-lookup"><span data-stu-id="88c01-128">Permissions to use the Custom Learning site as a user</span></span>

- <span data-ttu-id="88c01-129">Office 365 用户权限/SharePoint 网站访问者权限或更高权限</span><span class="sxs-lookup"><span data-stu-id="88c01-129">Office 365 user permissions/SharePoint Site Visitor permissions or higher</span></span>

## <a name="get-started-with-customization"></a><span data-ttu-id="88c01-130">自定义入门</span><span class="sxs-lookup"><span data-stu-id="88c01-130">Get started with customization</span></span>
<span data-ttu-id="88c01-131">确保拥有自定义网站和 web 部件所需的权限后, 即可开始使用自定义过程。</span><span class="sxs-lookup"><span data-stu-id="88c01-131">Once you've ensured you have the necessary permissions to customize the site and web part, it's time to get started with the customization process.</span></span> 

- <span data-ttu-id="88c01-132">若要开始, 请参阅[转到自定义学习网站](custom_goto.md)。</span><span class="sxs-lookup"><span data-stu-id="88c01-132">To get started, see [Go to the Custom Learning Site](custom_goto.md).</span></span>