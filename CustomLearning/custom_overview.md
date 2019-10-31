---
author: pkrebs
ms.author: pkrebs
title: 自定义学习路径
ms.date: 02/18/2019
description: 自定义学习路径
ms.openlocfilehash: 15d782455204cf043937bec03041a85abc9e4ee3
ms.sourcegitcommit: 3b8896c81ad2adbcfdbda658482847af5fccb264
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/30/2019
ms.locfileid: "37886635"
---
# <a name="customize-learning-pathways"></a><span data-ttu-id="9232d-103">自定义学习路径</span><span class="sxs-lookup"><span data-stu-id="9232d-103">Customize learning pathways</span></span>

<span data-ttu-id="9232d-104">Microsoft 365 学习途径提供了可用于为组织自定义内容的各种方法。</span><span class="sxs-lookup"><span data-stu-id="9232d-104">Microsoft 365 learning pathways provides a variety of ways that you can customize content for your organization.</span></span> <span data-ttu-id="9232d-105">例如，你能够：</span><span class="sxs-lookup"><span data-stu-id="9232d-105">For example, you can:</span></span>  
- <span data-ttu-id="9232d-106">修改 "SharePoint 网站" 的学习路径-更改网站名称、徽标和名称。</span><span class="sxs-lookup"><span data-stu-id="9232d-106">Modify the learning pathways SharePoint site - Change the site name, logo, and them.</span></span> <span data-ttu-id="9232d-107">修改 "提问" 和 "获取帮助" 页以创建您自己的帮助中心。</span><span class="sxs-lookup"><span data-stu-id="9232d-107">Modify the Ask Questions and Get Help page to create your own Help Center.</span></span> 
- <span data-ttu-id="9232d-108">隐藏或显示内容以反映组织中支持的服务或功能</span><span class="sxs-lookup"><span data-stu-id="9232d-108">Hide or show content to reflect the services or features supported in your organization</span></span> 
- <span data-ttu-id="9232d-109">专门针对用户需求构建自定义的播放列表和子类别</span><span class="sxs-lookup"><span data-stu-id="9232d-109">Build custom playlists and subcategories crafted specifically for your user's needs</span></span>
- <span data-ttu-id="9232d-110">使用经过筛选的内容生成登录页，以支持业务结果，例如促进 Microsoft 团队的采用、Outlook 移动或与 Microsoft 365 的协同工作。</span><span class="sxs-lookup"><span data-stu-id="9232d-110">Build landing pages with content filtered to support business outcomes, such as driving the adoption of Microsoft Teams, Outlook mobile, or working more collaboratively with Microsoft 365.</span></span>

![cg-introducing](media/cg-introducing.png)

## <a name="requirements-and-permissions"></a><span data-ttu-id="9232d-112">要求和权限</span><span class="sxs-lookup"><span data-stu-id="9232d-112">Requirements and Permissions</span></span>

<span data-ttu-id="9232d-113">在开始使用自定义学习路径指南之前，请确保已由 SharePoint 租户管理员设置了学习路径。</span><span class="sxs-lookup"><span data-stu-id="9232d-113">Before getting started with the Customize learning pathways guidance, ensure that learning pathways has been set up by your SharePoint Tenant Administrator.</span></span> <span data-ttu-id="9232d-114">如果您不确定是否已设置，请与您的 SharePoint 租户管理员联系，以验证是否已设置了学习路径。</span><span class="sxs-lookup"><span data-stu-id="9232d-114">If you’re not sure if it's been set up, contact your SharePoint tenant administrator to verify that learning pathways has been provisioned.</span></span> <span data-ttu-id="9232d-115">此外，请务必获取学习路径 SharePoint 网站的 URL。</span><span class="sxs-lookup"><span data-stu-id="9232d-115">Also be sure to get the URL of the learning pathways SharePoint site.</span></span> <span data-ttu-id="9232d-116">如果你是租户管理员，并且学习路径尚未设置，请参阅[设置学习路径](custom_provision.md)。</span><span class="sxs-lookup"><span data-stu-id="9232d-116">If you are the Tenant Administrator and learning pathways has not been provisioned, see [Provision learning pathways](custom_provision.md).</span></span> 

### <a name="permissions-to-provision-learning-pathways"></a><span data-ttu-id="9232d-117">设置学习路径的权限</span><span class="sxs-lookup"><span data-stu-id="9232d-117">Permissions to provision learning pathways</span></span>

- <span data-ttu-id="9232d-118">租户管理员，也称为 Office 365 全局管理员</span><span class="sxs-lookup"><span data-stu-id="9232d-118">Tenant Administrator, also known as Office 365 Global Administrator</span></span>
- <span data-ttu-id="9232d-119">具有网站所有者权限的 SharePoint 网站集管理员</span><span class="sxs-lookup"><span data-stu-id="9232d-119">SharePoint Site Collection Administrator with Owner permissions on the site</span></span>

### <a name="permissions-to-use-learning-pathways-administration-features"></a><span data-ttu-id="9232d-120">使用学习路径管理功能的权限</span><span class="sxs-lookup"><span data-stu-id="9232d-120">Permissions to use learning pathways Administration features</span></span>

- <span data-ttu-id="9232d-121">网站集管理员</span><span class="sxs-lookup"><span data-stu-id="9232d-121">Site Collection Administrator</span></span>
- <span data-ttu-id="9232d-122">SharePoint 所有者或成员权限</span><span class="sxs-lookup"><span data-stu-id="9232d-122">SharePoint Owner or Member permissions</span></span>

### <a name="permissions-to-use-the-learning-pathways-site-as-a-user"></a><span data-ttu-id="9232d-123">作为用户使用 "学习路径" 网站的权限</span><span class="sxs-lookup"><span data-stu-id="9232d-123">Permissions to use the learning pathways site as a user</span></span>

- <span data-ttu-id="9232d-124">Office 365 用户权限/SharePoint 网站访问者权限或更高权限</span><span class="sxs-lookup"><span data-stu-id="9232d-124">Office 365 user permissions/SharePoint Site Visitor permissions or higher</span></span>

## <a name="get-started-with-customization"></a><span data-ttu-id="9232d-125">自定义入门</span><span class="sxs-lookup"><span data-stu-id="9232d-125">Get started with customization</span></span>
<span data-ttu-id="9232d-126">确保拥有自定义网站和 web 部件所需的权限后，即可开始使用自定义过程。</span><span class="sxs-lookup"><span data-stu-id="9232d-126">Once you've ensured you have the necessary permissions to customize the site and web part, it's time to get started with the customization process.</span></span> 

- <span data-ttu-id="9232d-127">若要开始，请参阅[转到 "学习路径" 网站](custom_goto.md)。</span><span class="sxs-lookup"><span data-stu-id="9232d-127">To get started, see [Go to the learning pathways site](custom_goto.md).</span></span>