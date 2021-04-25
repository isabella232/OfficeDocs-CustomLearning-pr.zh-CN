---
author: pkrebs
ms.author: pkrebs
title: 自定义学习路径
ms.date: 02/18/2019
manager: bpardi
audience: admin
ms.topic: article
description: 自定义学习路径
ms.service: sharepoint-online
ms.openlocfilehash: a5087096ec3bd7c1194aab9dd089276fc196a736
ms.sourcegitcommit: 97e175e5ff5b6a9e0274d5ec9b39fdf7e18eb387
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/25/2021
ms.locfileid: "51999498"
---
# <a name="customize-learning-pathways"></a><span data-ttu-id="2e5cf-103">自定义学习路径</span><span class="sxs-lookup"><span data-stu-id="2e5cf-103">Customize learning pathways</span></span>

<span data-ttu-id="2e5cf-104">Microsoft 365 学习路径提供了多种方式，您可以为组织自定义内容。</span><span class="sxs-lookup"><span data-stu-id="2e5cf-104">Microsoft 365 learning pathways provides a variety of ways that you can customize content for your organization.</span></span> <span data-ttu-id="2e5cf-105">例如，你能够：</span><span class="sxs-lookup"><span data-stu-id="2e5cf-105">For example, you can:</span></span>  
- <span data-ttu-id="2e5cf-106">修改 SharePoint 网站的学习路径 - 更改网站名称、徽标及其。</span><span class="sxs-lookup"><span data-stu-id="2e5cf-106">Modify the learning pathways SharePoint site - Change the site name, logo, and them.</span></span> <span data-ttu-id="2e5cf-107">修改"提出问题并获取帮助"页以创建自己的帮助中心。</span><span class="sxs-lookup"><span data-stu-id="2e5cf-107">Modify the Ask Questions and Get Help page to create your own Help Center.</span></span> 
- <span data-ttu-id="2e5cf-108">隐藏或显示内容以反映组织支持的服务或功能</span><span class="sxs-lookup"><span data-stu-id="2e5cf-108">Hide or show content to reflect the services or features supported in your organization</span></span> 
- <span data-ttu-id="2e5cf-109">生成专为用户需求定制的自定义播放列表和子类别</span><span class="sxs-lookup"><span data-stu-id="2e5cf-109">Build custom playlists and subcategories crafted specifically for your user's needs</span></span>
- <span data-ttu-id="2e5cf-110">构建登录页面，其中的内容经过筛选以支持业务成果，例如推动 Microsoft Teams、Outlook 移动版或与 Microsoft 365 更协作地协作。</span><span class="sxs-lookup"><span data-stu-id="2e5cf-110">Build landing pages with content filtered to support business outcomes, such as driving the adoption of Microsoft Teams, Outlook mobile, or working more collaboratively with Microsoft 365.</span></span>

![常规 Microsoft 学习路径照片收集。](media/cg-introducing.png)

## <a name="requirements-and-permissions"></a><span data-ttu-id="2e5cf-112">要求和权限</span><span class="sxs-lookup"><span data-stu-id="2e5cf-112">Requirements and Permissions</span></span>

<span data-ttu-id="2e5cf-113">在开始使用自定义学习路径指南之前，请确保学习路径已由 SharePoint 租户管理员设置。</span><span class="sxs-lookup"><span data-stu-id="2e5cf-113">Before getting started with the Customize learning pathways guidance, ensure that learning pathways has been set up by your SharePoint Tenant Administrator.</span></span> <span data-ttu-id="2e5cf-114">如果不确定是否设置了，请与 SharePoint 租户管理员联系，以确认已预配学习路径。</span><span class="sxs-lookup"><span data-stu-id="2e5cf-114">If you’re not sure if it's been set up, contact your SharePoint tenant administrator to verify that learning pathways has been provisioned.</span></span> <span data-ttu-id="2e5cf-115">此外，请务必获取 SharePoint 网站的学习路径 URL。</span><span class="sxs-lookup"><span data-stu-id="2e5cf-115">Also be sure to get the URL of the learning pathways SharePoint site.</span></span> <span data-ttu-id="2e5cf-116">如果你是租户管理员，并且尚未设置学习路径，请参阅预配 [学习路径](custom_provision.md)。</span><span class="sxs-lookup"><span data-stu-id="2e5cf-116">If you are the Tenant Administrator and learning pathways has not been provisioned, see [Provision learning pathways](custom_provision.md).</span></span> 

### <a name="permissions-to-provision-learning-pathways"></a><span data-ttu-id="2e5cf-117">设置学习路径的权限</span><span class="sxs-lookup"><span data-stu-id="2e5cf-117">Permissions to provision learning pathways</span></span>

- <span data-ttu-id="2e5cf-118">租户管理员，也称为 Office 365 全局管理员</span><span class="sxs-lookup"><span data-stu-id="2e5cf-118">Tenant Administrator, also known as Office 365 Global Administrator</span></span>
- <span data-ttu-id="2e5cf-119">具有网站所有者权限的 SharePoint 网站集管理员</span><span class="sxs-lookup"><span data-stu-id="2e5cf-119">SharePoint Site Collection Administrator with Owner permissions on the site</span></span>

### <a name="permissions-to-use-learning-pathways-administration-features"></a><span data-ttu-id="2e5cf-120">使用学习路径的权限 管理功能</span><span class="sxs-lookup"><span data-stu-id="2e5cf-120">Permissions to use learning pathways Administration features</span></span>

- <span data-ttu-id="2e5cf-121">网站集管理员</span><span class="sxs-lookup"><span data-stu-id="2e5cf-121">Site Collection Administrator</span></span>
- <span data-ttu-id="2e5cf-122">SharePoint 所有者或成员权限</span><span class="sxs-lookup"><span data-stu-id="2e5cf-122">SharePoint Owner or Member permissions</span></span>

### <a name="permissions-to-use-the-learning-pathways-site-as-a-user"></a><span data-ttu-id="2e5cf-123">以用户方式使用学习路径网站的权限</span><span class="sxs-lookup"><span data-stu-id="2e5cf-123">Permissions to use the learning pathways site as a user</span></span>

- <span data-ttu-id="2e5cf-124">Office 365 用户权限/SharePoint 网站访问者权限或更高</span><span class="sxs-lookup"><span data-stu-id="2e5cf-124">Office 365 user permissions/SharePoint Site Visitor permissions or higher</span></span>

## <a name="get-started-with-customization"></a><span data-ttu-id="2e5cf-125">开始自定义设置</span><span class="sxs-lookup"><span data-stu-id="2e5cf-125">Get started with customization</span></span>
<span data-ttu-id="2e5cf-126">在确保你拥有自定义网站和 Web 部件所需的权限后，可以开始自定义过程了。</span><span class="sxs-lookup"><span data-stu-id="2e5cf-126">Once you've ensured you have the necessary permissions to customize the site and web part, it's time to get started with the customization process.</span></span> 

- <span data-ttu-id="2e5cf-127">若要开始，请参阅 [转到学习路径网站](custom_goto.md)。</span><span class="sxs-lookup"><span data-stu-id="2e5cf-127">To get started, see [Go to the learning pathways site](custom_goto.md).</span></span>