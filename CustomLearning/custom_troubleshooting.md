---
author: pkrebs
ms.author: pkrebs
title: Microsoft 365 学习路径故障排除
ms.date: 02/10/2019
description: 了解如何解决 Microsoft 365 学习路径问题
ms.service: sharepoint-online
manager: bpardi
ms.topic: article
audience: admin
ms.openlocfilehash: 7190688d574042c8a1b8dfb67c8b246dfbf8c927
ms.sourcegitcommit: 97e175e5ff5b6a9e0274d5ec9b39fdf7e18eb387
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/25/2021
ms.locfileid: "52000298"
---
# <a name="troubleshoot-microsoft-365-learning-pathways"></a><span data-ttu-id="56e5f-103">Microsoft 365 学习路径疑难解答</span><span class="sxs-lookup"><span data-stu-id="56e5f-103">Troubleshoot Microsoft 365 learning pathways</span></span>

<span data-ttu-id="56e5f-104">以下是有关 Microsoft 365 学习路径或 SharePoint Online 预配服务中可能存在的问题的疑难解答提示。</span><span class="sxs-lookup"><span data-stu-id="56e5f-104">Here are troubleshooting tips for problems that may occur with Microsoft 365 learning pathways or the SharePoint Online Provisioning Service.</span></span>

## <a name="how-to-know-if-you-have-tenant-admin-permissions"></a><span data-ttu-id="56e5f-105">如何知道您是否具有租户管理员权限</span><span class="sxs-lookup"><span data-stu-id="56e5f-105">How to know if you have Tenant Admin permissions</span></span>

<span data-ttu-id="56e5f-106">登录 SharePoint Online 预配服务并预配自定义学习需要租户管理员权限。</span><span class="sxs-lookup"><span data-stu-id="56e5f-106">Sign in to the SharePoint Online Provisioning Service and provisioning Custom Learning requires Tenant Admin permissions.</span></span> <span data-ttu-id="56e5f-107">如果遇到 SharePoint Online 预配服务的登录问题，请确保已分配有全局管理员角色。</span><span class="sxs-lookup"><span data-stu-id="56e5f-107">If you are experiencing sign in issues with the SharePoint Online Provisioning Service, make sure that you have been assigned the Global administrator role.</span></span> <span data-ttu-id="56e5f-108">自定义学习解决方案需要租户管理员权限，也称为 Office 365 全局管理员角色。</span><span class="sxs-lookup"><span data-stu-id="56e5f-108">The Custom Learning solution requires Tenant Admin permissions, otherwise known as Office 365 Global Administrator role.</span></span> <span data-ttu-id="56e5f-109">下面是如何确定是否分配了全局管理员角色。</span><span class="sxs-lookup"><span data-stu-id="56e5f-109">Here’s how to determine if you have been assigned the Global Administrator role.</span></span>

1.  <span data-ttu-id="56e5f-110">登录到 Office.com。</span><span class="sxs-lookup"><span data-stu-id="56e5f-110">Sign in to Office.com.</span></span>
2.  <span data-ttu-id="56e5f-111">单击 **"管理员"**</span><span class="sxs-lookup"><span data-stu-id="56e5f-111">Click **Admin**</span></span>
3.  <span data-ttu-id="56e5f-112">在 **"用户"** 下，选择 **"活动用户"**</span><span class="sxs-lookup"><span data-stu-id="56e5f-112">Under **Users**, select **Active Users**</span></span>
4.  <span data-ttu-id="56e5f-113">搜索你的姓名</span><span class="sxs-lookup"><span data-stu-id="56e5f-113">Search for your name</span></span>
5.  <span data-ttu-id="56e5f-114">在搜索结果中单击你的姓名。</span><span class="sxs-lookup"><span data-stu-id="56e5f-114">Click your name in Search results.</span></span> <span data-ttu-id="56e5f-115">应看到角色的全局管理员。</span><span class="sxs-lookup"><span data-stu-id="56e5f-115">You should see Global administrator for your role.</span></span>
<span data-ttu-id="56e5f-116">![列出角色以及许可证、组成员身份和其他信息的示例页面。](media/cg-globaladminrole.png)</span><span class="sxs-lookup"><span data-stu-id="56e5f-116">![Sample page that lists your role along with licenses, group memberships and other information.](media/cg-globaladminrole.png)</span></span>

### <a name="if-you-dont-have-the-global-administrator-role"></a><span data-ttu-id="56e5f-117">如果你没有全局管理员角色</span><span class="sxs-lookup"><span data-stu-id="56e5f-117">If you don’t have the Global administrator role</span></span>
- <span data-ttu-id="56e5f-118">在组织中查找全局管理员，让此人登录该服务或让他们分配全局管理员角色。</span><span class="sxs-lookup"><span data-stu-id="56e5f-118">Find a Global Administrator in your organization and have that person sign into the service or have them assign the Global administrator role to you.</span></span>

## <a name="tenant-app-catalog-troubleshooting"></a><span data-ttu-id="56e5f-119">租户应用程序目录疑难解答</span><span class="sxs-lookup"><span data-stu-id="56e5f-119">Tenant App Catalog Troubleshooting</span></span>
<span data-ttu-id="56e5f-120">自定义学习需要在目标租户中预配应用程序目录。</span><span class="sxs-lookup"><span data-stu-id="56e5f-120">Custom Learning requires an App Catalog to be provisioned in the target tenant.</span></span> <span data-ttu-id="56e5f-121">创建应用程序目录需要全局管理员权限。</span><span class="sxs-lookup"><span data-stu-id="56e5f-121">Creating an app catalog requires Global Administrator permissions.</span></span> <span data-ttu-id="56e5f-122">以下是常见应用程序目录问题的疑难解答步骤：</span><span class="sxs-lookup"><span data-stu-id="56e5f-122">Here’s are troubleshooting steps for common App Catalog issues:</span></span>

### <a name="how-to-know-if-you-have-a-tenant-app-catalog"></a><span data-ttu-id="56e5f-123">如何知道您是否具有租户应用程序目录</span><span class="sxs-lookup"><span data-stu-id="56e5f-123">How to know if you have a Tenant app catalog</span></span> 
<span data-ttu-id="56e5f-124">对于初学者，请确保你拥有全局管理员权限。</span><span class="sxs-lookup"><span data-stu-id="56e5f-124">For starters, ensure that you have Global administrator permissions.</span></span> <span data-ttu-id="56e5f-125">请参阅上述租户管理员权限的步骤。</span><span class="sxs-lookup"><span data-stu-id="56e5f-125">See the steps for Tenant Admin permissions above.</span></span>

1. <span data-ttu-id="56e5f-126">From Office 365， click **Admin**， click the expand arrow >， click **Show all**  >  **Admin centers**  >  **SharePoint**.</span><span class="sxs-lookup"><span data-stu-id="56e5f-126">From Office 365, click **Admin**, click the expand arrow >, click **Show all** > **Admin centers** > **SharePoint**.</span></span>
2. <span data-ttu-id="56e5f-127">单击 **经典管理 SharePoint 中心**  >  **应用程序**  >  **应用程序目录**。</span><span class="sxs-lookup"><span data-stu-id="56e5f-127">Click **Classic Admin SharePoint Center** > **apps** > **App Catalog**.</span></span>
3. <span data-ttu-id="56e5f-128">在 **"应用程序**"下，应看到标题为"分发 **SharePoint 应用程序"的磁贴**。</span><span class="sxs-lookup"><span data-stu-id="56e5f-128">Under **Apps**, you should see a tile titled **Distribute apps for SharePoint**.</span></span> <span data-ttu-id="56e5f-129">如果你看到此磁贴，则你有一个租户应用程序目录。</span><span class="sxs-lookup"><span data-stu-id="56e5f-129">If you see the tile, you have a Tenant App Catalog.</span></span> <span data-ttu-id="56e5f-130">请参阅 **下面的如何确保你是网站集合...** 部分。</span><span class="sxs-lookup"><span data-stu-id="56e5f-130">See the **How to ensure your are a Site Colllection...** section below.</span></span> <span data-ttu-id="56e5f-131">如果看不到磁贴，则需要为租户创建租户应用目录。</span><span class="sxs-lookup"><span data-stu-id="56e5f-131">If you don’t see the tile you will need to create a tenant app catalog for your tenant.</span></span> <span data-ttu-id="56e5f-132">请参阅 **下面的如何创建租户应用程序目录** 部分。</span><span class="sxs-lookup"><span data-stu-id="56e5f-132">See the **How to create a Tenant App Catalog** section below .</span></span>

### <a name="how-to-ensure-you-are-a-site-collection-owner-on-the-tenant-app-catalog"></a><span data-ttu-id="56e5f-133">如何确保你是租户应用程序目录中的网站集所有者</span><span class="sxs-lookup"><span data-stu-id="56e5f-133">How to ensure you are a Site Collection Owner on the Tenant App Catalog</span></span> 
<span data-ttu-id="56e5f-134">若要预配 Microsoft 365 学习路径，你需要是租户应用目录中的网站集所有者。</span><span class="sxs-lookup"><span data-stu-id="56e5f-134">To provision Microsoft 365 learning pathways, you will need to be a Site Collection Owner on the Tenant App Catalog.</span></span> <span data-ttu-id="56e5f-135">下面将了解如何确定您是否为所有者。</span><span class="sxs-lookup"><span data-stu-id="56e5f-135">Here’s how to determine if you are an Owner.</span></span>

1. <span data-ttu-id="56e5f-136">From Office 365， click **Admin**， click the expand arrow >， click **Show all**  >  **Admin centers**  >  **SharePoint**.</span><span class="sxs-lookup"><span data-stu-id="56e5f-136">From Office 365, click **Admin**, click the expand arrow >, click **Show all** > **Admin centers** > **SharePoint**.</span></span>
2. <span data-ttu-id="56e5f-137">单击 **"经典管理 SharePoint 中心**"，然后选择 **应用程序目录**。</span><span class="sxs-lookup"><span data-stu-id="56e5f-137">Click **Classic Admin SharePoint Center**, and then select the **app catalog**.</span></span>
3. <span data-ttu-id="56e5f-138">选择 **"** 所有者"，然后确保您是网站集所有者。</span><span class="sxs-lookup"><span data-stu-id="56e5f-138">Select **Owner**, and then ensure you are a Site Collection Owner.</span></span> <span data-ttu-id="56e5f-139">它应如下所示。</span><span class="sxs-lookup"><span data-stu-id="56e5f-139">It should look something like this.</span></span>
<span data-ttu-id="56e5f-140">!["管理管理员"页。](media/cg-sitecollectionowner.png)</span><span class="sxs-lookup"><span data-stu-id="56e5f-140">![Manage administrators page.](media/cg-sitecollectionowner.png)</span></span>

### <a name="how-to-create-a-tenant-app-catalog-if-one-doesnt-exists"></a><span data-ttu-id="56e5f-141">如何创建租户应用程序目录（如果不存在）</span><span class="sxs-lookup"><span data-stu-id="56e5f-141">How to create a Tenant App Catalog if one doesn’t exists</span></span> 
1. <span data-ttu-id="56e5f-142">使用 SharePoint Online 管理员帐户登录 Office 365。</span><span class="sxs-lookup"><span data-stu-id="56e5f-142">Sign in to Office 365 with your SharePoint Online admin account.</span></span>
2. <span data-ttu-id="56e5f-143">单击“**管理员**”。</span><span class="sxs-lookup"><span data-stu-id="56e5f-143">Click **Admin**.</span></span>
3. <span data-ttu-id="56e5f-144">在"**管理中心"下**，单击 **"SharePoint"。**</span><span class="sxs-lookup"><span data-stu-id="56e5f-144">Under **Admin centers**, click **SharePoint**.</span></span> 
4. <span data-ttu-id="56e5f-145">单击 **应用程序**  >  **应用程序目录**。</span><span class="sxs-lookup"><span data-stu-id="56e5f-145">Click **Apps** > **App Catalog**.</span></span>
5. <span data-ttu-id="56e5f-146">单击 **"新建应用程序目录网站"，** 然后单击"确定 **"。**</span><span class="sxs-lookup"><span data-stu-id="56e5f-146">Click **Create a new app catalog site**, and then click **OK**.</span></span> 
6.  <span data-ttu-id="56e5f-147">输入应用程序目录的信息。</span><span class="sxs-lookup"><span data-stu-id="56e5f-147">Enter the information for the App Catalog.</span></span> <span data-ttu-id="56e5f-148">您可能需要包括多个管理员。</span><span class="sxs-lookup"><span data-stu-id="56e5f-148">You may want to include more than one Administrator.</span></span> <span data-ttu-id="56e5f-149">下面显示了一个示例。</span><span class="sxs-lookup"><span data-stu-id="56e5f-149">The following shows an example.</span></span>  
![用于输入新应用程序目录信息的表单。](media/cg-appcatalogfinish.png)

7.  <span data-ttu-id="56e5f-151">就是这样。</span><span class="sxs-lookup"><span data-stu-id="56e5f-151">That’s it.</span></span> <span data-ttu-id="56e5f-152">已完成。</span><span class="sxs-lookup"><span data-stu-id="56e5f-152">You’re done.</span></span> <span data-ttu-id="56e5f-153">但在设置自定义学习之前，你需要等待至少 30 分钟，以确保应用程序目录创建完成。</span><span class="sxs-lookup"><span data-stu-id="56e5f-153">But before you move to provisioning Custom Learning, you need to wait at least 30 minutes to make sure the App Catalog creation is complete.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="56e5f-154">在创建租户应用程序目录后至少等待 30 分钟，然后再预配自定义学习。</span><span class="sxs-lookup"><span data-stu-id="56e5f-154">Wait at least 30 minutes after creating the Tenant App Catalog before provisioning Custom Learning.</span></span> <span data-ttu-id="56e5f-155">这将确保应用程序目录预配过程在 SharePoint 中完成。</span><span class="sxs-lookup"><span data-stu-id="56e5f-155">This ensures that the App Catalog provisioning process is complete within SharePoint.</span></span> 