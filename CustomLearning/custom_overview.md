---
author: pkrebs
ms.author: pkrebs
title: 概述
ms.date: 02/18/2019
description: Microsoft 365 学习路径概述
ms.openlocfilehash: 74fac090177ad8009155e21a977b05ee2b742b3b
ms.sourcegitcommit: f5a7079d56598c14aef2f4b886c025a59ba89276
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/21/2019
ms.locfileid: "34247839"
---
# <a name="customize-the-learning-experience"></a><span data-ttu-id="d439d-103">自定义学习体验</span><span class="sxs-lookup"><span data-stu-id="d439d-103">Customize the learning experience</span></span>

<span data-ttu-id="d439d-104">Microsoft 365 学习途径简介，Microsoft 旨在加快组织内部使用和采用 Office 365 的新解决方案。</span><span class="sxs-lookup"><span data-stu-id="d439d-104">Introducing Microsoft 365 learning pathways, a new solution from Microsoft designed to speed the usage and adoption of Office 365 within an organization.</span></span> <span data-ttu-id="d439d-105">通过学习 pathwyas，您可以：</span><span class="sxs-lookup"><span data-stu-id="d439d-105">With learning pathwyas, you can:</span></span>
- <span data-ttu-id="d439d-106">为您的环境定制 Microsoft 365 学习和采用内容</span><span class="sxs-lookup"><span data-stu-id="d439d-106">Tailor Microsoft 365 learning and adoption content for your environment</span></span> 
- <span data-ttu-id="d439d-107">隐藏或显示内容以反映组织中支持的服务或功能</span><span class="sxs-lookup"><span data-stu-id="d439d-107">Hide or show content to reflect the services or features supported in your organization</span></span> 
- <span data-ttu-id="d439d-108">使用 Microsoft 提供最新的学习内容，让你的内容和用户保持最新的订阅源</span><span class="sxs-lookup"><span data-stu-id="d439d-108">Keep your content and users current with an up-to-date feed of learning content from Microsoft</span></span> 
- <span data-ttu-id="d439d-109">专门针对用户需求构建自定义的播放列表和类别</span><span class="sxs-lookup"><span data-stu-id="d439d-109">Build custom playlists and categories crafted specifically for your user's needs</span></span>

![cg-introducing](media/cg-introducing.png)

## <a name="how-does-learning-pathways-work"></a><span data-ttu-id="d439d-111">学习路径的工作原理是什么？</span><span class="sxs-lookup"><span data-stu-id="d439d-111">How does learning pathways work?</span></span>

<span data-ttu-id="d439d-112">Office 365 的学习路径（简短的学习路径）包括三个部分：</span><span class="sxs-lookup"><span data-stu-id="d439d-112">learning pathways for Office 365 (learning pathways for short) consists of three parts:</span></span> 
1. <span data-ttu-id="d439d-113">Microsoft online 目录中的内容的实时订阅源</span><span class="sxs-lookup"><span data-stu-id="d439d-113">a live feed of content from a Microsoft online catalog</span></span>
2. <span data-ttu-id="d439d-114">SharePoint 通信网站</span><span class="sxs-lookup"><span data-stu-id="d439d-114">a SharePoint communication site</span></span>
3. <span data-ttu-id="d439d-115">SharePoint web 部件</span><span class="sxs-lookup"><span data-stu-id="d439d-115">a SharePoint web part</span></span> 

![cg-howitworks](media/cg-howitworks.png)

## <a name="requirements-and-permissions"></a><span data-ttu-id="d439d-117">要求和权限</span><span class="sxs-lookup"><span data-stu-id="d439d-117">Requirements and Permissions</span></span>

<span data-ttu-id="d439d-118">在开始使用本指南之前，请确保已由 SharePoint 租户管理员设置了学习路径。</span><span class="sxs-lookup"><span data-stu-id="d439d-118">Before getting started with this guide, ensure that learning pathways has been set up by your SharePoint Tenant Administrator.</span></span> <span data-ttu-id="d439d-119">如果您不确定是否已设置，请与您的 SharePoint 租户管理员联系，以验证是否已设置了学习路径。</span><span class="sxs-lookup"><span data-stu-id="d439d-119">If you’re not sure if it's been set up, contact your SharePoint tenant administrator to verify that learning pathways has been provisioned.</span></span> <span data-ttu-id="d439d-120">此外，请务必获取学习路径 SharePoint 网站的 URL。</span><span class="sxs-lookup"><span data-stu-id="d439d-120">Also be sure to get the URL of the learning pathways SharePoint site.</span></span> <span data-ttu-id="d439d-121">如果你是租户管理员，并且学习路径尚未设置，请参阅[设置学习路径](custom_provision.md)。</span><span class="sxs-lookup"><span data-stu-id="d439d-121">If you are the Tenant Administrator and learning pathways has not been provisioned, see [Provision learning pathways](custom_provision.md).</span></span> 

### <a name="permissions-to-provision-learning-pathways"></a><span data-ttu-id="d439d-122">设置学习路径的权限</span><span class="sxs-lookup"><span data-stu-id="d439d-122">Permissions to provision learning pathways</span></span>

- <span data-ttu-id="d439d-123">租户管理员，也称为 Office 365 全局管理员</span><span class="sxs-lookup"><span data-stu-id="d439d-123">Tenant Administrator, also known as Office 365 Global Administrator</span></span>
- <span data-ttu-id="d439d-124">具有网站所有者权限的 SharePoint 网站集管理员</span><span class="sxs-lookup"><span data-stu-id="d439d-124">SharePoint Site Collection Administrator with Owner permissions on the site</span></span>

### <a name="permissions-to-use-learning-pathways-administration-features"></a><span data-ttu-id="d439d-125">使用学习路径管理功能的权限</span><span class="sxs-lookup"><span data-stu-id="d439d-125">Permissions to use learning pathways Administration features</span></span>

- <span data-ttu-id="d439d-126">网站集管理员</span><span class="sxs-lookup"><span data-stu-id="d439d-126">Site Collection Administrator</span></span>
- <span data-ttu-id="d439d-127">SharePoint 所有者或成员权限</span><span class="sxs-lookup"><span data-stu-id="d439d-127">SharePoint Owner or Member permissions</span></span>

### <a name="permissions-to-use-the-learning-pathways-site-as-a-user"></a><span data-ttu-id="d439d-128">作为用户使用 "学习路径" 网站的权限</span><span class="sxs-lookup"><span data-stu-id="d439d-128">Permissions to use the learning pathways site as a user</span></span>

- <span data-ttu-id="d439d-129">Office 365 用户权限/SharePoint 网站访问者权限或更高权限</span><span class="sxs-lookup"><span data-stu-id="d439d-129">Office 365 user permissions/SharePoint Site Visitor permissions or higher</span></span>

## <a name="get-started-with-customization"></a><span data-ttu-id="d439d-130">自定义入门</span><span class="sxs-lookup"><span data-stu-id="d439d-130">Get started with customization</span></span>
<span data-ttu-id="d439d-131">确保拥有自定义网站和 web 部件所需的权限后，即可开始使用自定义过程。</span><span class="sxs-lookup"><span data-stu-id="d439d-131">Once you've ensured you have the necessary permissions to customize the site and web part, it's time to get started with the customization process.</span></span> 

- <span data-ttu-id="d439d-132">若要开始，请参阅[转到 "学习路径" 网站](custom_goto.md)。</span><span class="sxs-lookup"><span data-stu-id="d439d-132">To get started, see [Go to the learning pathways site](custom_goto.md).</span></span>