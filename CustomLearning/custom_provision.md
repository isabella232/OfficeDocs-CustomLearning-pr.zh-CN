---
author: pkrebs
ms.author: pkrebs
title: 预配自定义学习网站
ms.date: 02/10/2019
description: 通过 SharePoint 预配引擎为 Office 365 网站设置自定义学习
ms.openlocfilehash: 868708f9f096c84d5ebc5f9bc4e21e558da84d2b
ms.sourcegitcommit: 775d6807291ab263eea5ec649d9aaf1933fb41ca
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/23/2019
ms.locfileid: "32055875"
---
# <a name="provision-custom-learning"></a><span data-ttu-id="b0c47-103">预配自定义学习</span><span class="sxs-lookup"><span data-stu-id="b0c47-103">Provision Custom Learning</span></span> 

<span data-ttu-id="b0c47-104">借助 SharePoint Online 设置服务, Office 365 租户管理员可以通过几次简单的单击操作来启动预配过程。</span><span class="sxs-lookup"><span data-stu-id="b0c47-104">With the SharePoint Online Provisioning Service, an Office 365 Tenant Administrator can start the provisioning process with a few simple clicks.</span></span> <span data-ttu-id="b0c47-105">预配服务是设置自定义学习的推荐方法。</span><span class="sxs-lookup"><span data-stu-id="b0c47-105">The Provisioning Service is the recommended way to provision Custom Learning.</span></span> <span data-ttu-id="b0c47-106">快速而简单, 只需几分钟即可启动该过程。</span><span class="sxs-lookup"><span data-stu-id="b0c47-106">It's fast, easy, and takes only a few minutes to start the process.</span></span> <span data-ttu-id="b0c47-107">但是, 在开始使用预配服务之前, 请确保已满足预配的先决条件。</span><span class="sxs-lookup"><span data-stu-id="b0c47-107">Before getting started with the Provisioning Service, however, make sure you've met the prerequisites for provisioning.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b0c47-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b0c47-108">Prerequisites</span></span>
 
<span data-ttu-id="b0c47-109">若要使用预配服务成功设置自定义学习, 进行预配的人员必须满足以下先决条件:</span><span class="sxs-lookup"><span data-stu-id="b0c47-109">To successfully set up Custom Learning with the Provisioning Service, the person doing the provisioning must meet the following pre-requisites:</span></span> 
 
- <span data-ttu-id="b0c47-110">人员预配自定义学习必须是租户的租户管理员, 其中将预配自定义学习。</span><span class="sxs-lookup"><span data-stu-id="b0c47-110">The person provisioning Custom Learning must be a Tenant Administrator of the tenant where Custom Learning will be provisioned.</span></span>  
- <span data-ttu-id="b0c47-111">租户应用程序目录必须在 SharePoint 管理中心的 "应用程序" 选项中可用。</span><span class="sxs-lookup"><span data-stu-id="b0c47-111">A tenant App Catalog must be available within the Apps option of the SharePoint Admin Center.</span></span> <span data-ttu-id="b0c47-112">如果您的组织没有 SharePoint 租户应用程序目录, 请参阅[SharePoint Online 文档](https://docs.microsoft.com/en-us/sharepoint/use-app-catalog)以创建一个。</span><span class="sxs-lookup"><span data-stu-id="b0c47-112">If your organization does not have an SharePoint tenant App catalog, refer to the [SharePoint Online documentation](https://docs.microsoft.com/en-us/sharepoint/use-app-catalog) to create one.</span></span>  
- <span data-ttu-id="b0c47-113">人员预配自定义学习必须是租户应用程序目录的网站集所有者。</span><span class="sxs-lookup"><span data-stu-id="b0c47-113">The person provisioning Custom Learning must be a Site Collection Owner of the Tenant App Catalog.</span></span> <span data-ttu-id="b0c47-114">如果人员预配自定义学习不是应用程序目录的网站集所有者, 请[完成这些说明](addappadmin.md)并继续。</span><span class="sxs-lookup"><span data-stu-id="b0c47-114">If the person provisioning Custom Learning is not a Site Collection Owner of the App Catalog [complete these instructions](addappadmin.md) and continue.</span></span> 

### <a name="to-provision-custom-learning"></a><span data-ttu-id="b0c47-115">预配自定义学习</span><span class="sxs-lookup"><span data-stu-id="b0c47-115">To provision Custom Learning</span></span>

1. <span data-ttu-id="b0c47-116">从主页http://provisioning.sharepointpnp.com的右上角转到并**登录**。</span><span class="sxs-lookup"><span data-stu-id="b0c47-116">Go to http://provisioning.sharepointpnp.com and **sign in** from the upper right hand corner of the home page.</span></span>  <span data-ttu-id="b0c47-117">使用您计划安装网站模板的目标租户的凭据登录。</span><span class="sxs-lookup"><span data-stu-id="b0c47-117">Sign in with the  credentials for the targeted tenant where you plan to install the site template.</span></span>

![pnphome](media/inst_signin.png)

2. <span data-ttu-id="b0c47-119">清除**代表您的组织的同意**并选择 "**接受**"。</span><span class="sxs-lookup"><span data-stu-id="b0c47-119">Clear the **Consent on behalf of your organization** and select **Accept**.</span></span>

![实时](media/inst_perms.png)

3. <span data-ttu-id="b0c47-121">向下滚动页面, 选择 "**解决方案**" 选项卡, 然后选择 "**自定义 Office 365 的学习**"。</span><span class="sxs-lookup"><span data-stu-id="b0c47-121">Scroll down the page, select the **Solutions** tab, and then select **Custom learning for Office 365**.</span></span> 

![实时](media/inst_select.png)

4. <span data-ttu-id="b0c47-123">选择 "**添加到你的租户**"</span><span class="sxs-lookup"><span data-stu-id="b0c47-123">Select **Add to your tenant**</span></span>

![inst_select](media/inst_add.png)

5. <span data-ttu-id="b0c47-125">根据您的安装需要填写 "设置信息" 页上的字段。</span><span class="sxs-lookup"><span data-stu-id="b0c47-125">Complete the fields on the provisioning information page as appropriate for your installation.</span></span> <span data-ttu-id="b0c47-126">至少应输入你希望获取有关设置过程的通知的电子邮件地址和要设置为的网站的目标 URL。</span><span class="sxs-lookup"><span data-stu-id="b0c47-126">At a minimum enter the email address where you wish to get notifications about the provisioning process and the destination URL for your site to be provisioned to.</span></span>  
> [!NOTE]
> <span data-ttu-id="b0c47-127">将网站的目标 URL 设置为友好的内容, 如 "/sites/MyTraining" 或 "/teams/LearnOffice365"。</span><span class="sxs-lookup"><span data-stu-id="b0c47-127">Make the destination URL for your site something friendly to your employees such as "/sites/MyTraining" or "/teams/LearnOffice365".</span></span>

![inst_options](media/inst_options.png)

6. <span data-ttu-id="b0c47-129">准备好将自定义学习安装到租户环境中时, 请选择 "**设置**"。</span><span class="sxs-lookup"><span data-stu-id="b0c47-129">Select **Provision** when ready to install Custom Learning into your tenant environment.</span></span>  <span data-ttu-id="b0c47-130">预配过程最长需要15分钟。</span><span class="sxs-lookup"><span data-stu-id="b0c47-130">The provisioning process will take up to 15 minutes.</span></span> <span data-ttu-id="b0c47-131">当网站准备好访问时, 将通过电子邮件通知你 (到您在 "设置" 页上输入的通知电子邮件地址)。</span><span class="sxs-lookup"><span data-stu-id="b0c47-131">You will be notified via email (to the notification email address you entered on the Provisioning page) when the site is ready for access.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="b0c47-132">设置自定义学习网站的租户管理员必须转到网站, 然后打开**CustomLearningAdmin**以初始化自定义学习管理属性。</span><span class="sxs-lookup"><span data-stu-id="b0c47-132">The Tenant Admin who provisions the Custom Learning site must go to the site, and then open **CustomLearningAdmin.aspx** to initialize Custom Learning Admin properties.</span></span> <span data-ttu-id="b0c47-133">目前, 租户管理员还应将所有者分配给网站。</span><span class="sxs-lookup"><span data-stu-id="b0c47-133">At this time, the Tenant Admin should also assign Owners to the site.</span></span> 

## <a name="validate-provisioning-success-and-initialize-the-customconfig-list"></a><span data-ttu-id="b0c47-134">验证设置是否成功并初始化 CustomConfig 列表</span><span class="sxs-lookup"><span data-stu-id="b0c47-134">Validate Provisioning Success and Initialize the CustomConfig List</span></span>

<span data-ttu-id="b0c47-135">设置完成后, 预配网站的租户管理员会收到来自 PnP 预配服务的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="b0c47-135">When provisioning is complete, the Tenant Admin who provisioned the site, receives an email from the PnP Provisioning Service.</span></span> <span data-ttu-id="b0c47-136">电子邮件包含指向该网站的链接。</span><span class="sxs-lookup"><span data-stu-id="b0c47-136">The email contains a link to the site.</span></span> <span data-ttu-id="b0c47-137">在这种情况下, 租户管理员应使用电子邮件中提供的链接转到网站, 并将网站设置为首次使用:</span><span class="sxs-lookup"><span data-stu-id="b0c47-137">At this point, the Tenant Admin should go to the site using the link provided in the email and set up the site for first use:</span></span>

- <span data-ttu-id="b0c47-138">转到 `<YOUR-SITE-COLLECTION-URL>sites/<YOUR-SITE-NAME>/SitePages/CustomLearningAdmin.aspx`。</span><span class="sxs-lookup"><span data-stu-id="b0c47-138">Go to `<YOUR-SITE-COLLECTION-URL>sites/<YOUR-SITE-NAME>/SitePages/CustomLearningAdmin.aspx`.</span></span> <span data-ttu-id="b0c47-139">打开**CustomLearningAdmin**可初始化**CustomConfig**列表项, 该列表项设置自定义学习以供首次使用。</span><span class="sxs-lookup"><span data-stu-id="b0c47-139">Opening **CustomLearningAdmin.aspx** initializes the **CustomConfig** list item that sets up Custom Learning for first use.</span></span> <span data-ttu-id="b0c47-140">您应该会看到如下所示的页面:</span><span class="sxs-lookup"><span data-stu-id="b0c47-140">You should see a page that looks like this:</span></span>

![cg-adminapppage](media/cg-adminapppage.png)

## <a name="add-owners-to-site"></a><span data-ttu-id="b0c47-142">将所有者添加到网站</span><span class="sxs-lookup"><span data-stu-id="b0c47-142">Add Owners to Site</span></span>
<span data-ttu-id="b0c47-143">作为租户管理员, 您不太可能是自定义网站的人员, 因此您需要向网站分配一些所有者。</span><span class="sxs-lookup"><span data-stu-id="b0c47-143">As the Tenant Admin, it's unlikely you'll be the person customizing the site, so you'll need to assign a few owners to the site.</span></span> <span data-ttu-id="b0c47-144">所有者具有对网站的管理权限, 以便他们可以修改网站页面并 rebrand 网站。</span><span class="sxs-lookup"><span data-stu-id="b0c47-144">Owners have administrative privileges on the site so they can modify site pages and rebrand the site.</span></span> <span data-ttu-id="b0c47-145">他们还能够隐藏和显示通过自定义学习 Web 部件传递的内容。</span><span class="sxs-lookup"><span data-stu-id="b0c47-145">They also have the ability to hide and show content delivered through the Custom Learning Web part.</span></span> <span data-ttu-id="b0c47-146">此外, 他们还能够构建自定义播放列表并将其分配给自定义子类别。</span><span class="sxs-lookup"><span data-stu-id="b0c47-146">In addition, they'll have the ability to build custom playlist and assign them to custom subcategories.</span></span>  

1. <span data-ttu-id="b0c47-147">从 "SharePoint**设置**" 菜单中, 单击 "**网站权限**"。</span><span class="sxs-lookup"><span data-stu-id="b0c47-147">From the SharePoint **Settings** menu, click **Site Permissions**.</span></span>
2. <span data-ttu-id="b0c47-148">单击 "**高级权限设置**"。</span><span class="sxs-lookup"><span data-stu-id="b0c47-148">Click **Advanced Permission Settings**.</span></span>
3. <span data-ttu-id="b0c47-149">单击 "**自定义学习 for Office 365 所有者**"。</span><span class="sxs-lookup"><span data-stu-id="b0c47-149">Click **Custom learning for Office 365 Owners**.</span></span>
4. <span data-ttu-id="b0c47-150">单击 "**新建** > 向**此组添加用户**", 然后添加您希望成为所有者的人员。</span><span class="sxs-lookup"><span data-stu-id="b0c47-150">Click **New** > **Add Users to this group**, and then add the people you want to be Owners.</span></span> 
5. <span data-ttu-id="b0c47-151">添加链接以在共享邮件中[浏览网站](custom_exploresite.md), 然后单击 "**共享**"。</span><span class="sxs-lookup"><span data-stu-id="b0c47-151">Add a link to [Explore the Site](custom_exploresite.md) in the Share message, and then click **Share**.</span></span>

### <a name="next-steps"></a><span data-ttu-id="b0c47-152">后续步骤</span><span class="sxs-lookup"><span data-stu-id="b0c47-152">Next Steps</span></span>
- <span data-ttu-id="b0c47-153">浏览网站和 web 部件中提供的[默认内容](custom_exploresite.md)。</span><span class="sxs-lookup"><span data-stu-id="b0c47-153">Explore the [default content](custom_exploresite.md) provided in the site and web part.</span></span>
