---
author: pkrebs
ms.author: pkrebs
title: Microsoft 365 学习途径故障排除
ms.date: 02/10/2019
description: 了解如何对 Microsoft 365 学习路径进行故障排除
ms.openlocfilehash: de46b9c754dac36de230b36ec4a5542518a1dcd5
ms.sourcegitcommit: 1a111a49a0413a56a880e29109ba01b5e5f33d09
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/20/2019
ms.locfileid: "34247677"
---
# <a name="troubleshoot-microsoft-365-learning-pathways"></a><span data-ttu-id="04119-103">解决 Microsoft 365 学习路径问题</span><span class="sxs-lookup"><span data-stu-id="04119-103">Troubleshoot Microsoft 365 learning pathways</span></span>

<span data-ttu-id="04119-104">下面是在 Microsoft 365 学习通道或 SharePoint Online 设置服务中可能出现的问题的故障排除提示。</span><span class="sxs-lookup"><span data-stu-id="04119-104">Here are troubleshooting tips for problems that may occur with Microsoft 365 learning pathways or the SharePoint Online Provisioning Service.</span></span>

## <a name="how-to-know-if-you-have-tenant-admin-permissions"></a><span data-ttu-id="04119-105">如何知道你是否拥有租户管理员权限</span><span class="sxs-lookup"><span data-stu-id="04119-105">How to know if you have Tenant Admin permissions</span></span>

<span data-ttu-id="04119-106">登录到 SharePoint Online 设置服务并设置自定义学习需要租户管理员权限。</span><span class="sxs-lookup"><span data-stu-id="04119-106">Sign in to the SharePoint Online Provisioning Service and provisioning Custom Learning requires Tenant Admin permissions.</span></span> <span data-ttu-id="04119-107">如果您在使用 SharePoint Online 设置服务时遇到登录问题, 请确保已为您分配全局管理员角色。</span><span class="sxs-lookup"><span data-stu-id="04119-107">If you are experiencing sign in issues with the SharePoint Online Provisioning Service, make sure that you have been assigned the Global administrator role.</span></span> <span data-ttu-id="04119-108">自定义学习解决方案需要租户管理员权限, 否则称为 Office 365 全局管理员角色。</span><span class="sxs-lookup"><span data-stu-id="04119-108">The Custom Learning solution requires Tenant Admin permissions, otherwise known as Office 365 Global Administrator role.</span></span> <span data-ttu-id="04119-109">下面介绍了如何确定是否已向你分配全局管理员角色。</span><span class="sxs-lookup"><span data-stu-id="04119-109">Here’s how to determine if you have been assigned the Global Administrator role.</span></span>

1.  <span data-ttu-id="04119-110">登录到 Office.com。</span><span class="sxs-lookup"><span data-stu-id="04119-110">Sign in to Office.com.</span></span>
2.  <span data-ttu-id="04119-111">单击 "**管理**"</span><span class="sxs-lookup"><span data-stu-id="04119-111">Click **Admin**</span></span>
3.  <span data-ttu-id="04119-112">在 "**用户**" 下, 选择 "**活动用户**"</span><span class="sxs-lookup"><span data-stu-id="04119-112">Under **Users**, select **Active Users**</span></span>
4.  <span data-ttu-id="04119-113">搜索您的姓名</span><span class="sxs-lookup"><span data-stu-id="04119-113">Search for your name</span></span>
5.  <span data-ttu-id="04119-114">在搜索结果中单击您的姓名。</span><span class="sxs-lookup"><span data-stu-id="04119-114">Click your name in Search results.</span></span> <span data-ttu-id="04119-115">您应看到您的角色的全局管理员。</span><span class="sxs-lookup"><span data-stu-id="04119-115">You should see Global administrator for your role.</span></span>

![cg-globaladminrole](media/cg-globaladminrole.png)

### <a name="if-you-dont-have-the-global-administrator-role"></a><span data-ttu-id="04119-117">如果你没有全局管理员角色</span><span class="sxs-lookup"><span data-stu-id="04119-117">If you don’t have the Global administrator role</span></span>
- <span data-ttu-id="04119-118">在您的组织中查找全局管理员, 并让该用户登录到该服务, 或让其为您分配全局管理员角色。</span><span class="sxs-lookup"><span data-stu-id="04119-118">Find a Global Administrator in your organization and have that person sign into the service or have them assign the Global administrator role to you.</span></span>

## <a name="tenant-app-catalog-troubleshooting"></a><span data-ttu-id="04119-119">租户应用程序目录故障排除</span><span class="sxs-lookup"><span data-stu-id="04119-119">Tenant App Catalog Troubleshooting</span></span>
<span data-ttu-id="04119-120">自定义学习要求在目标租户中预配应用程序目录。</span><span class="sxs-lookup"><span data-stu-id="04119-120">Custom Learning requires an App Catalog to be provisioned in the target tenant.</span></span> <span data-ttu-id="04119-121">创建应用程序目录需要全局管理员权限。</span><span class="sxs-lookup"><span data-stu-id="04119-121">Creating an app catalog requires Global Administrator permissions.</span></span> <span data-ttu-id="04119-122">下面是常见应用程序目录问题的故障排除步骤:</span><span class="sxs-lookup"><span data-stu-id="04119-122">Here’s are troubleshooting steps for common App Catalog issues:</span></span>

### <a name="how-to-know-if-you-have-a-tenant-app-catalog"></a><span data-ttu-id="04119-123">如何知道你是否拥有租户应用目录</span><span class="sxs-lookup"><span data-stu-id="04119-123">How to know if you have a Tenant app catalog</span></span> 
<span data-ttu-id="04119-124">对于初学者, 请确保您具有全局管理员权限。</span><span class="sxs-lookup"><span data-stu-id="04119-124">For starters, ensure that you have Global administrator permissions.</span></span> <span data-ttu-id="04119-125">请参阅上述租户管理员权限的步骤。</span><span class="sxs-lookup"><span data-stu-id="04119-125">See the steps for Tenant Admin permissions above.</span></span>

1. <span data-ttu-id="04119-126">从 Office 365 中, 单击 "**管理**", 单击 "展开" 箭头 >, 单击 "**显示所有** > **管理中心** > **SharePoint**"。</span><span class="sxs-lookup"><span data-stu-id="04119-126">From Office 365, click **Admin**, click the expand arrow >, click **Show all** > **Admin centers** > **SharePoint**.</span></span>
2. <span data-ttu-id="04119-127">单击 "**经典管理 SharePoint 中心** > **应用** > **程序目录**"。</span><span class="sxs-lookup"><span data-stu-id="04119-127">Click **Classic Admin SharePoint Center** > **apps** > **App Catalog**.</span></span>
3. <span data-ttu-id="04119-128">在 "**应用程序**" 下, 应看到一个标有 "**分布 SharePoint 相关应用程序**" 的磁贴</span><span class="sxs-lookup"><span data-stu-id="04119-128">Under **Apps**, you should see a tile titled **Distribute apps for SharePoint**.</span></span> <span data-ttu-id="04119-129">如果您看到磁贴, 则您有租户应用程序目录。</span><span class="sxs-lookup"><span data-stu-id="04119-129">If you see the tile, you have a Tenant App Catalog.</span></span> <span data-ttu-id="04119-130">请参阅下面的**如何确保你是网站 Colllection ...** 部分。</span><span class="sxs-lookup"><span data-stu-id="04119-130">See the **How to ensure your are a Site Colllection...** section below.</span></span> <span data-ttu-id="04119-131">如果看不到磁贴, 你将需要为租户创建租户应用目录。</span><span class="sxs-lookup"><span data-stu-id="04119-131">If you don’t see the tile you will need to create a tenant app catalog for your tenant.</span></span> <span data-ttu-id="04119-132">请参阅下面的**如何创建租户应用目录**部分。</span><span class="sxs-lookup"><span data-stu-id="04119-132">See the **How to create a Tenant App Catalog** section below .</span></span>

### <a name="how-to-ensure-you-are-a-site-collection-owner-on-the-tenant-app-catalog"></a><span data-ttu-id="04119-133">如何确保你是租户应用程序目录上的网站集所有者</span><span class="sxs-lookup"><span data-stu-id="04119-133">How to ensure you are a Site Collection Owner on the Tenant App Catalog</span></span> 
<span data-ttu-id="04119-134">若要设置 Microsoft 365 学习路径, 您需要是租户应用程序目录上的网站集所有者。</span><span class="sxs-lookup"><span data-stu-id="04119-134">To provision Microsoft 365 learning pathways, you will need to be a Site Collection Owner on the Tenant App Catalog.</span></span> <span data-ttu-id="04119-135">下面介绍如何确定你是否为所有者。</span><span class="sxs-lookup"><span data-stu-id="04119-135">Here’s how to determine if you are an Owner.</span></span>

1. <span data-ttu-id="04119-136">从 Office 365 中, 单击 "**管理**", 单击 "展开" 箭头 >, 单击 "**显示所有** > **管理中心** > **SharePoint**"。</span><span class="sxs-lookup"><span data-stu-id="04119-136">From Office 365, click **Admin**, click the expand arrow >, click **Show all** > **Admin centers** > **SharePoint**.</span></span>
2. <span data-ttu-id="04119-137">单击 "**经典管理 SharePoint 中心**", 然后选择 "**应用程序目录**"。</span><span class="sxs-lookup"><span data-stu-id="04119-137">Click **Classic Admin SharePoint Center**, and then select the **app catalog**.</span></span>
3. <span data-ttu-id="04119-138">选择 "**所有者**", 然后确保您是网站集所有者。</span><span class="sxs-lookup"><span data-stu-id="04119-138">Select **Owner**, and then ensure you are a Site Collection Owner.</span></span> <span data-ttu-id="04119-139">它应类似于以下内容。</span><span class="sxs-lookup"><span data-stu-id="04119-139">It should look something like this.</span></span>
 
![cg-sitecollectionowner](media/cg-sitecollectionowner.png)

### <a name="how-to-create-a-tenant-app-catalog-if-one-doesnt-exists"></a><span data-ttu-id="04119-141">如何创建租户应用程序目录 (如果不存在)</span><span class="sxs-lookup"><span data-stu-id="04119-141">How to create a Tenant App Catalog if one doesn’t exists</span></span> 
1. <span data-ttu-id="04119-142">使用您的 SharePoint Online 管理员帐户登录到 Office 365。</span><span class="sxs-lookup"><span data-stu-id="04119-142">Sign in to Office 365 with your SharePoint Online admin account.</span></span>
2. <span data-ttu-id="04119-143">单击“**管理员**”。</span><span class="sxs-lookup"><span data-stu-id="04119-143">Click **Admin**.</span></span>
3. <span data-ttu-id="04119-144">在 "**管理中心**" 下, 单击 " **SharePoint**"。</span><span class="sxs-lookup"><span data-stu-id="04119-144">Under **Admin centers**, click **SharePoint**.</span></span> 
4. <span data-ttu-id="04119-145">单击 "**应用** > "**应用程序目录**。</span><span class="sxs-lookup"><span data-stu-id="04119-145">Click **Apps** > **App Catalog**.</span></span>
5. <span data-ttu-id="04119-146">单击 "**新建应用程序目录网站**", 然后单击 **"确定"**。</span><span class="sxs-lookup"><span data-stu-id="04119-146">Click **Create a new app catalog site**, and then click **OK**.</span></span> 
6.  <span data-ttu-id="04119-147">输入应用程序目录的信息。</span><span class="sxs-lookup"><span data-stu-id="04119-147">Enter the information for the App Catalog.</span></span> <span data-ttu-id="04119-148">您可能想要包含多个管理员。</span><span class="sxs-lookup"><span data-stu-id="04119-148">You may want to include more than one Administrator.</span></span> <span data-ttu-id="04119-149">下面显示了一个示例。</span><span class="sxs-lookup"><span data-stu-id="04119-149">The following shows an example.</span></span>  

![cg-appcatalogfinish](media/cg-appcatalogfinish.png)

7.  <span data-ttu-id="04119-151">就是这样。</span><span class="sxs-lookup"><span data-stu-id="04119-151">That’s it.</span></span> <span data-ttu-id="04119-152">已经完成。</span><span class="sxs-lookup"><span data-stu-id="04119-152">You’re done.</span></span> <span data-ttu-id="04119-153">但在迁移到预配自定义学习之前, 至少需要等待30分钟, 才能确保应用程序目录创建已完成。</span><span class="sxs-lookup"><span data-stu-id="04119-153">But before you move to provisioning Custom Learning, you need to wait at least 30 minutes to make sure the App Catalog creation is complete.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="04119-154">创建租户应用程序目录后至少等待30分钟, 然后再设置自定义学习。</span><span class="sxs-lookup"><span data-stu-id="04119-154">Wait at least 30 minutes after creating the Tenant App Catalog before provisioning Custom Learning.</span></span> <span data-ttu-id="04119-155">这可确保应用程序目录设置过程在 SharePoint 中完成。</span><span class="sxs-lookup"><span data-stu-id="04119-155">This ensures that the App Catalog provisioning process is complete within SharePoint.</span></span> 