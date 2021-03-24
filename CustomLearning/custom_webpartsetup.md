---
author: pkrebs
ms.author: pkrebs
title: 设置自定义学习网站
ms.date: 02/10/2019
description: 通过 SharePoint 预配引擎预配 Office 365 自定义学习网站
ms.service: sharepoint online
ms.openlocfilehash: be45ade7588f08801062710d310ca967ddd23926
ms.sourcegitcommit: 907c657e7cc5a4a44d2b9f38cc35fea9ac5c5943
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/24/2021
ms.locfileid: "51162919"
---
# <a name="provision-custom-learning"></a><span data-ttu-id="67e8e-103">预配自定义学习</span><span class="sxs-lookup"><span data-stu-id="67e8e-103">Provision Custom Learning</span></span>

<span data-ttu-id="67e8e-104">借助 SharePoint Online 预配服务，Office 365 租户管理员可以通过单击几下即可开始预配过程。</span><span class="sxs-lookup"><span data-stu-id="67e8e-104">With the SharePoint Online Provisioning Service, an Office 365 Tenant Administrator can start the provisioning process with a few simple clicks.</span></span> <span data-ttu-id="67e8e-105">预配服务是设置自定义学习的推荐方法。</span><span class="sxs-lookup"><span data-stu-id="67e8e-105">The Provisioning Service is the recommended way to provision Custom Learning.</span></span> <span data-ttu-id="67e8e-106">它快速、简单，只需几分钟即可开始该过程。</span><span class="sxs-lookup"><span data-stu-id="67e8e-106">It's fast, easy, and takes only a few minutes to start the process.</span></span> <span data-ttu-id="67e8e-107">但是，在开始使用预配服务之前，请确保你已满足预配的先决条件。</span><span class="sxs-lookup"><span data-stu-id="67e8e-107">Before getting started with the Provisioning Service, however, make sure you've met the prerequisites for provisioning.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="67e8e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="67e8e-108">Prerequisites</span></span>
 
<span data-ttu-id="67e8e-109">若要使用设置服务 [SharePoint Online 设置](https://provisioning.sharepointpnp.com)服务成功设置自定义学习，执行预配的人必须满足以下先决条件：</span><span class="sxs-lookup"><span data-stu-id="67e8e-109">To successfully set up Custom Learning with the Provisioning Service [SharePoint Online Provisioning Service](https://provisioning.sharepointpnp.com), the person doing the provisioning must meet the following pre-requisites:</span></span> 
 
- <span data-ttu-id="67e8e-110">预配自定义学习的人必须是将预配自定义学习的租户的租户管理员。</span><span class="sxs-lookup"><span data-stu-id="67e8e-110">The person provisioning Custom Learning must be a Tenant Administratorof the tenant where Custom Learning will be provisioned.</span></span>  
- <span data-ttu-id="67e8e-111">租户应用程序目录必须在 SharePoint 管理中心的"应用程序"选项中提供。</span><span class="sxs-lookup"><span data-stu-id="67e8e-111">A tenant App Catalog must be available within the Apps option of the SharePoint Admin Center.</span></span> <span data-ttu-id="67e8e-112">如果您的组织没有 SharePoint 租户应用程序目录，请参阅 [SharePoint Online 文档以](/sharepoint/use-app-catalog) 创建一个。</span><span class="sxs-lookup"><span data-stu-id="67e8e-112">If your organization does not have an SharePoint tenant App catalog, refer to the [SharePoint Online documentation](/sharepoint/use-app-catalog) to create one.</span></span>  
- <span data-ttu-id="67e8e-113">预配自定义学习的人必须是租户应用程序目录的网站集所有者。</span><span class="sxs-lookup"><span data-stu-id="67e8e-113">The person provisioning Custom Learning must be a Site Collection Owner of the Tenant App Catalog.</span></span> <span data-ttu-id="67e8e-114">如果预配自定义学习的人不是应用程序目录的网站集所有者，请 [完成这些说明并继续](addappadmin.md) 操作。</span><span class="sxs-lookup"><span data-stu-id="67e8e-114">If the person provisioning Custom Learning is not a Site Collection Owner of the App Catalog [complete these instructions](addappadmin.md) and continue.</span></span> 

### <a name="to-provision-custom-learning"></a><span data-ttu-id="67e8e-115">设置自定义学习</span><span class="sxs-lookup"><span data-stu-id="67e8e-115">To provision Custom Learning</span></span>

1. <span data-ttu-id="67e8e-116">转到 http://provisioning.sharepointpnp.com **，然后** 从主页的右上角登录。</span><span class="sxs-lookup"><span data-stu-id="67e8e-116">Go to http://provisioning.sharepointpnp.com and **sign in** from the upper right hand corner of the home page.</span></span>  <span data-ttu-id="67e8e-117">使用计划安装网站模板的目标租户的凭据登录。</span><span class="sxs-lookup"><span data-stu-id="67e8e-117">Sign in with the  credentials for the targeted tenant where you plan to install the site template.</span></span>

![pnphome.png](media/inst_signin.png)

2. <span data-ttu-id="67e8e-119">清除"**代表你的组织同意"，然后选择**"接受 **"。**</span><span class="sxs-lookup"><span data-stu-id="67e8e-119">Clear the **Consent on behalf of your organization** and select **Accept**.</span></span>

![属于 ](media/inst_perms.png)

3. <span data-ttu-id="67e8e-121">从 **解决方案库中选择"自定义学习 office 365"。**</span><span class="sxs-lookup"><span data-stu-id="67e8e-121">Select **Custom Learning for Office 365** from the solution gallery.</span></span>

![属于 ](media/inst_select.png)

4. <span data-ttu-id="67e8e-123">从解决方案主页选择" **添加到租户"**</span><span class="sxs-lookup"><span data-stu-id="67e8e-123">From the solution home page select **Add to your Tenant**</span></span>

![inst_select.png](media/inst_add.png)

5. <span data-ttu-id="67e8e-125">根据需要填写预配信息页面上的字段。</span><span class="sxs-lookup"><span data-stu-id="67e8e-125">Complete the fields on the provisioning information page as appropriate for your installation.</span></span> <span data-ttu-id="67e8e-126">至少输入要获取预配过程通知的电子邮件地址，以及要预配到的网站的目标 URL。</span><span class="sxs-lookup"><span data-stu-id="67e8e-126">At a minimum enter the email address where you wish to get notifications about the provisioning process and the destination URL for your site to be provisioned to.</span></span>  
> [!NOTE]
> <span data-ttu-id="67e8e-127">使网站的目标 URL 对员工友好，例如"/sites/MyTraining"或"/teams/LearnOffice365"。</span><span class="sxs-lookup"><span data-stu-id="67e8e-127">Make the destination URL for your site something friendly to your employees such as "/sites/MyTraining" or "/teams/LearnOffice365".</span></span>

![inst_options.png](media/inst_options.png)

6. <span data-ttu-id="67e8e-129">准备好 **将** 自定义学习安装到租户环境中时，请选择"预配"。</span><span class="sxs-lookup"><span data-stu-id="67e8e-129">Select **Provision** when ready to install Custom Learning into your tenant environment.</span></span>  <span data-ttu-id="67e8e-130">预配流程最多需要 15 分钟。</span><span class="sxs-lookup"><span data-stu-id="67e8e-130">The provisioning process will take up to 15 minutes.</span></span> <span data-ttu-id="67e8e-131">网站可供访问时，系统将通过电子邮件（你在“预配”页面上输入的通知电子邮件地址）通知你。</span><span class="sxs-lookup"><span data-stu-id="67e8e-131">You will be notified via email (to the notification email address you entered on the Provisioning page) when the site is ready for access.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="67e8e-132">设置自定义学习网站的租户管理员必须转到该网站，然后打开 CustomLearningAdmin.aspx 以初始化自定义学习管理员属性。</span><span class="sxs-lookup"><span data-stu-id="67e8e-132">The Tenant Admin who provisions the Custom Learning site must go to the site, and then open CustomLearningAdmin.aspx to initialize Custom Learning Admin properties.</span></span> <span data-ttu-id="67e8e-133">目前，租户管理员还应将所有者分配给网站。</span><span class="sxs-lookup"><span data-stu-id="67e8e-133">At this time, the Tenant Admin should also assign Owners to the site.</span></span> 

## <a name="validate-provisioning-success"></a><span data-ttu-id="67e8e-134">验证预配成功</span><span class="sxs-lookup"><span data-stu-id="67e8e-134">Validate Provisioning Success</span></span>

<span data-ttu-id="67e8e-135">预配完成后，租户管理员将收到来自 PnP 预配服务的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="67e8e-135">When provisioning is complete, the Tenant Admin receives an email from the PnP Provisioning Service.</span></span> <span data-ttu-id="67e8e-136">管理员可以将链接复制到电子邮件中提供的网站，然后按照说明转到网站。</span><span class="sxs-lookup"><span data-stu-id="67e8e-136">The admin can copy the link to the site provided in the email, and then follow the instructions to go to the site.</span></span> <span data-ttu-id="67e8e-137">或者，租户管理员可以导航到 </SitePages/CustomLearningAdmin.aspx>YOUR-SITE-COLLECTION-URL。</span><span class="sxs-lookup"><span data-stu-id="67e8e-137">Alternately, the tenant admin can navigate to <YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx.</span></span> <span data-ttu-id="67e8e-138">这将初始化 CustomConfig 列表项，该列表项将设置自定义学习供其首次使用。</span><span class="sxs-lookup"><span data-stu-id="67e8e-138">This initializes the CustomConfig list item that sets up Custom Learning for its first use.</span></span> <span data-ttu-id="67e8e-139">第一次打开此页面的用户必须是租户管理员、网站集管理员或网站所有者。</span><span class="sxs-lookup"><span data-stu-id="67e8e-139">The person who first opens this page must be a Tenant Admin,Site Collection Admin, or Owner of the site.</span></span> <span data-ttu-id="67e8e-140">应看到如下页面：</span><span class="sxs-lookup"><span data-stu-id="67e8e-140">You should see a page that looks like this:</span></span> 

## <a name="add-owners-to-site"></a><span data-ttu-id="67e8e-141">将所有者添加到网站</span><span class="sxs-lookup"><span data-stu-id="67e8e-141">Add Owners to Site</span></span>
<span data-ttu-id="67e8e-142">作为租户管理员，你不太可能是自定义网站的人，因此你需要将所有者分配给网站。</span><span class="sxs-lookup"><span data-stu-id="67e8e-142">As the Tenant Admin, it's unlikely you'll be the person customizing the site, so you'll need to assign Owners to the site.</span></span> <span data-ttu-id="67e8e-143">所有者对网站拥有管理权限，因此可以修改网站页面和重新品牌。</span><span class="sxs-lookup"><span data-stu-id="67e8e-143">Owners have administrative privileges on the site so they can modify site pages and rebrand the site.</span></span> <span data-ttu-id="67e8e-144">他们还能够隐藏和显示通过自定义学习 Web 部件提供的内容。</span><span class="sxs-lookup"><span data-stu-id="67e8e-144">They also have the ability to hide and show content delivered through the Custom Learning Web part.</span></span> <span data-ttu-id="67e8e-145">他们还可以生成自定义播放列表并将其分配给自定义子类别。</span><span class="sxs-lookup"><span data-stu-id="67e8e-145">They'll also have the ability to build custom playlist and assign them to custom subcategories.</span></span>  

1. <span data-ttu-id="67e8e-146">从"SharePoint **设置"菜单中**，单击"**网站权限"。**</span><span class="sxs-lookup"><span data-stu-id="67e8e-146">From the SharePoint **Settings** menu, click **Site Permissions**.</span></span>
2. <span data-ttu-id="67e8e-147">单击 **"高级权限设置"。**</span><span class="sxs-lookup"><span data-stu-id="67e8e-147">Click **Advanced Permission Settings**.</span></span>
3. <span data-ttu-id="67e8e-148">单击 **Office 365 所有者的自定义学习**。</span><span class="sxs-lookup"><span data-stu-id="67e8e-148">Click **Custom learning for Office 365 Owners**.</span></span>
4. <span data-ttu-id="67e8e-149">单击 **"**  >  **向此组添加新用户"，** 添加您希望成为所有者的用户，然后单击"共享 **"。**</span><span class="sxs-lookup"><span data-stu-id="67e8e-149">Click **New** > **Add Users to this group**, add the people you want to be Owners, and then click **Share**.</span></span>

8. <span data-ttu-id="67e8e-150">单击 **页面** 右上角的"关注"选项以关注网站。</span><span class="sxs-lookup"><span data-stu-id="67e8e-150">Click the **Following** option in the upper right hand corner of the page to follow the site.</span></span>  

### <a name="next-steps"></a><span data-ttu-id="67e8e-151">后续步骤</span><span class="sxs-lookup"><span data-stu-id="67e8e-151">Next Steps</span></span>
- <span data-ttu-id="67e8e-152">浏览 [Web 部件](sitecontent.md) 中包含的默认内容。</span><span class="sxs-lookup"><span data-stu-id="67e8e-152">Explore the [default content](sitecontent.md) included in the webpart.</span></span>