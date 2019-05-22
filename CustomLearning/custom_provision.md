---
author: pkrebs
ms.author: pkrebs
title: 预配 Microsoft 365 学习路径网站
ms.date: 02/10/2019
description: 通过 SharePoint 设置服务设置 Microsoft 365 学习路径网站
ms.openlocfilehash: e48052a395a8669ef684110a1c93409f5859a1d2
ms.sourcegitcommit: 0077704d7edcc26eda76900115716fc5b7b1c518
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2019
ms.locfileid: "34334737"
---
# <a name="provision-microsoft-365-learning-pathways"></a><span data-ttu-id="71eb1-103">预配 Microsoft 365 学习路径</span><span class="sxs-lookup"><span data-stu-id="71eb1-103">Provision Microsoft 365 learning pathways</span></span>

<span data-ttu-id="71eb1-104">借助 SharePoint Online 设置服务, Office 365 租户管理员可以通过几次简单的单击操作来启动预配过程。</span><span class="sxs-lookup"><span data-stu-id="71eb1-104">With the SharePoint Online Provisioning Service, an Office 365 Tenant Administrator can start the provisioning process with a few simple clicks.</span></span> <span data-ttu-id="71eb1-105">预配服务是设置学习路径的推荐方法。</span><span class="sxs-lookup"><span data-stu-id="71eb1-105">The Provisioning Service is the recommended way to provision learning pathways.</span></span> <span data-ttu-id="71eb1-106">快速而简单, 只需几分钟即可启动该过程。</span><span class="sxs-lookup"><span data-stu-id="71eb1-106">It's fast, easy, and takes only a few minutes to start the process.</span></span> <span data-ttu-id="71eb1-107">但是, 在开始使用预配服务之前, 请确保已满足预配的先决条件。</span><span class="sxs-lookup"><span data-stu-id="71eb1-107">Before getting started with the Provisioning Service, however, make sure you've met the prerequisites for provisioning.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="71eb1-108">从5/21/2019 到, Microsoft 365 学习途径是以前称为 "Office 365 自定义学习" 的解决方案的新名称。</span><span class="sxs-lookup"><span data-stu-id="71eb1-108">As of 5/21/2019, Microsoft 365 learning pathways is the new name for the solution formerly known as Custom Learning for Office 365.</span></span> <span data-ttu-id="71eb1-109">如果已为组织中的 Office 365 设置了自定义学习, 并且想要更新解决方案, 请按照[Microsoft 365 学习途径自述文件](https://github.com/pnp/custom-learning-office-365)中的 "更新解决方案" 说明操作。</span><span class="sxs-lookup"><span data-stu-id="71eb1-109">If you have already provisioned Custom Learning for Office 365 in your organization and want to update the solution, follow the “Updating the solution” instructions in the [Microsoft 365 learning pathways ReadMe](https://github.com/pnp/custom-learning-office-365).</span></span> <span data-ttu-id="71eb1-110">如果您是首次预配 Microsoft 365 学习路径, 请参阅 Microsoft 365 学习通道文档中的[预配 microsoft 365 学习通道说明]( https://docs.microsoft.com/en-us/office365/customlearning/custom_provision)。</span><span class="sxs-lookup"><span data-stu-id="71eb1-110">If you are provisioning Microsoft 365 learning pathways for the first time, see [Provision Microsoft 365 learning pathways instructions]( https://docs.microsoft.com/en-us/office365/customlearning/custom_provision) in the Microsoft 365 learning pathways documentation.</span></span>  

## <a name="prerequisites"></a><span data-ttu-id="71eb1-111">先决条件</span><span class="sxs-lookup"><span data-stu-id="71eb1-111">Prerequisites</span></span>
 
<span data-ttu-id="71eb1-112">若要成功设置与预配服务的 Microsoft 365 学习路径, 执行预配的人员必须满足以下先决条件:</span><span class="sxs-lookup"><span data-stu-id="71eb1-112">To successfully set up Microsoft 365 learning pathways with the Provisioning Service, the person doing the provisioning must meet the following pre-requisites:</span></span> 
 
- <span data-ttu-id="71eb1-113">人员预配学习路径必须是租户的租户管理员, 其中将预配学习路径。</span><span class="sxs-lookup"><span data-stu-id="71eb1-113">The person provisioning learning pathways must be a Tenant Administrator of the tenant where learning pathways will be provisioned.</span></span>  
- <span data-ttu-id="71eb1-114">租户应用程序目录必须在 SharePoint 管理中心的 "应用程序" 选项中可用。</span><span class="sxs-lookup"><span data-stu-id="71eb1-114">A tenant App Catalog must be available within the Apps option of the SharePoint Admin Center.</span></span> <span data-ttu-id="71eb1-115">如果您的组织没有 SharePoint 租户应用程序目录, 请参阅[SharePoint Online 文档](https://docs.microsoft.com/en-us/sharepoint/use-app-catalog)以创建一个。</span><span class="sxs-lookup"><span data-stu-id="71eb1-115">If your organization does not have an SharePoint tenant App catalog, refer to the [SharePoint Online documentation](https://docs.microsoft.com/en-us/sharepoint/use-app-catalog) to create one.</span></span>  
- <span data-ttu-id="71eb1-116">人员预配学习路径必须是租户应用程序目录的网站集所有者。</span><span class="sxs-lookup"><span data-stu-id="71eb1-116">The person provisioning learning pathways must be a Site Collection Owner of the Tenant App Catalog.</span></span> <span data-ttu-id="71eb1-117">如果人员设置学习路径不是应用程序目录的网站集所有者, 请[完成这些说明](addappadmin.md)并继续。</span><span class="sxs-lookup"><span data-stu-id="71eb1-117">If the person provisioning learning pathways is not a Site Collection Owner of the App Catalog [complete these instructions](addappadmin.md) and continue.</span></span> 

### <a name="to-provision-learning-pathways"></a><span data-ttu-id="71eb1-118">设置学习路径</span><span class="sxs-lookup"><span data-stu-id="71eb1-118">To provision learning pathways</span></span>

1. <span data-ttu-id="71eb1-119">从主页http://provisioning.sharepointpnp.com的右上角转到并**登录**。</span><span class="sxs-lookup"><span data-stu-id="71eb1-119">Go to http://provisioning.sharepointpnp.com and **sign in** from the upper right hand corner of the home page.</span></span>  <span data-ttu-id="71eb1-120">使用您计划安装网站模板的目标租户的凭据登录。</span><span class="sxs-lookup"><span data-stu-id="71eb1-120">Sign in with the  credentials for the targeted tenant where you plan to install the site template.</span></span>

![pnphome](media/inst_signin.png)

2. <span data-ttu-id="71eb1-122">清除**代表您的组织的同意**并选择 "**接受**"。</span><span class="sxs-lookup"><span data-stu-id="71eb1-122">Clear the **Consent on behalf of your organization** and select **Accept**.</span></span>

![实时](media/inst_perms.png)

<span data-ttu-id="71eb1-124">预配服务需要这些权限才能创建租户应用程序目录, 请将应用程序安装到租户应用目录中并预配网站模板。</span><span class="sxs-lookup"><span data-stu-id="71eb1-124">The provisioning service requires these permissions to create the tenant app catalog, install the application into the tenant app catalog and provision the site template.</span></span> <span data-ttu-id="71eb1-125">对租户没有整体影响, 并且这些权限将显式用于解决方案安装的目的。</span><span class="sxs-lookup"><span data-stu-id="71eb1-125">There is no overall impact on your tenant and these permissions are explicitly used for the purpose of the solution installation.</span></span> <span data-ttu-id="71eb1-126">您必须接受这些权限才能继续安装。</span><span class="sxs-lookup"><span data-stu-id="71eb1-126">You must accept these permissions to proceed with the installation.</span></span>

3. <span data-ttu-id="71eb1-127">向下滚动页面, 选择 "**解决方案**" 选项卡, 然后选择 " **Office 365 的学习路径**"。</span><span class="sxs-lookup"><span data-stu-id="71eb1-127">Scroll down the page, select the **Solutions** tab, and then select **learning pathways for Office 365**.</span></span> 

![实时](media/inst_select.png)

4. <span data-ttu-id="71eb1-129">选择 "**添加到你的租户**"</span><span class="sxs-lookup"><span data-stu-id="71eb1-129">Select **Add to your tenant**</span></span>

![inst_select](media/inst_add.png)

5. <span data-ttu-id="71eb1-131">根据您的安装需要填写 "设置信息" 页上的字段。</span><span class="sxs-lookup"><span data-stu-id="71eb1-131">Complete the fields on the provisioning information page as appropriate for your installation.</span></span> <span data-ttu-id="71eb1-132">至少应输入你希望获取有关设置过程的通知的电子邮件地址和要设置为的网站的目标 URL。</span><span class="sxs-lookup"><span data-stu-id="71eb1-132">At a minimum enter the email address where you wish to get notifications about the provisioning process and the destination URL for your site to be provisioned to.</span></span>  
> [!NOTE]
> <span data-ttu-id="71eb1-133">将网站的目标 URL 设置为友好的内容, 如 "/sites/MyTraining" 或 "/teams/LearnMicrosoft365"。</span><span class="sxs-lookup"><span data-stu-id="71eb1-133">Make the destination URL for your site something friendly to your employees such as "/sites/MyTraining" or "/teams/LearnMicrosoft365".</span></span>

![inst_options](media/inst_options.png)

6. <span data-ttu-id="71eb1-135">准备好将学习路径安装到你的租户环境中时, 请选择 "**设置**"。</span><span class="sxs-lookup"><span data-stu-id="71eb1-135">Select **Provision** when ready to install learning pathways into your tenant environment.</span></span>  <span data-ttu-id="71eb1-136">预配过程最长需要15分钟。</span><span class="sxs-lookup"><span data-stu-id="71eb1-136">The provisioning process will take up to 15 minutes.</span></span> <span data-ttu-id="71eb1-137">当网站准备好访问时, 将通过电子邮件通知你 (到您在 "设置" 页上输入的通知电子邮件地址)。</span><span class="sxs-lookup"><span data-stu-id="71eb1-137">You will be notified via email (to the notification email address you entered on the Provisioning page) when the site is ready for access.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="71eb1-138">预配学习路径网站的租户管理员必须转到网站, 然后打开**CustomLearningAdmin**以初始化 "学习路径管理" 属性。</span><span class="sxs-lookup"><span data-stu-id="71eb1-138">The Tenant Admin who provisions the learning pathways site must go to the site, and then open **CustomLearningAdmin.aspx** to initialize learning pathways Admin properties.</span></span> <span data-ttu-id="71eb1-139">目前, 租户管理员还应将所有者分配给网站。</span><span class="sxs-lookup"><span data-stu-id="71eb1-139">At this time, the Tenant Admin should also assign Owners to the site.</span></span> 

## <a name="validate-provisioning-success-and-initialize-the-customconfig-list"></a><span data-ttu-id="71eb1-140">验证设置是否成功并初始化 CustomConfig 列表</span><span class="sxs-lookup"><span data-stu-id="71eb1-140">Validate Provisioning Success and Initialize the CustomConfig List</span></span>

<span data-ttu-id="71eb1-141">设置完成后, 预配网站的租户管理员会收到来自 PnP 预配服务的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="71eb1-141">When provisioning is complete, the Tenant Admin who provisioned the site, receives an email from the PnP Provisioning Service.</span></span> <span data-ttu-id="71eb1-142">电子邮件包含指向该网站的链接。</span><span class="sxs-lookup"><span data-stu-id="71eb1-142">The email contains a link to the site.</span></span> <span data-ttu-id="71eb1-143">在这种情况下, 租户管理员应使用电子邮件中提供的链接转到网站, 并将网站设置为首次使用:</span><span class="sxs-lookup"><span data-stu-id="71eb1-143">At this point, the Tenant Admin should go to the site using the link provided in the email and set up the site for first use:</span></span>

- <span data-ttu-id="71eb1-144">转到 `<YOUR-SITE-COLLECTION-URL>sites/<YOUR-SITE-NAME>/SitePages/CustomLearningAdmin.aspx`。</span><span class="sxs-lookup"><span data-stu-id="71eb1-144">Go to `<YOUR-SITE-COLLECTION-URL>sites/<YOUR-SITE-NAME>/SitePages/CustomLearningAdmin.aspx`.</span></span> <span data-ttu-id="71eb1-145">打开**CustomLearningAdmin**可初始化**CustomConfig**列表项, 该列表项设置首次使用的学习路径。</span><span class="sxs-lookup"><span data-stu-id="71eb1-145">Opening **CustomLearningAdmin.aspx** initializes the **CustomConfig** list item that sets up learning pathways for first use.</span></span> <span data-ttu-id="71eb1-146">您应该会看到如下所示的页面:</span><span class="sxs-lookup"><span data-stu-id="71eb1-146">You should see a page that looks like this:</span></span>

![cg-adminapppage](media/cg-adminapppage.png)

## <a name="add-owners-to-site"></a><span data-ttu-id="71eb1-148">将所有者添加到网站</span><span class="sxs-lookup"><span data-stu-id="71eb1-148">Add Owners to Site</span></span>
<span data-ttu-id="71eb1-149">作为租户管理员, 您不太可能是自定义网站的人员, 因此您需要向网站分配一些所有者。</span><span class="sxs-lookup"><span data-stu-id="71eb1-149">As the Tenant Admin, it's unlikely you'll be the person customizing the site, so you'll need to assign a few owners to the site.</span></span> <span data-ttu-id="71eb1-150">所有者具有对网站的管理权限, 以便他们可以修改网站页面并 rebrand 网站。</span><span class="sxs-lookup"><span data-stu-id="71eb1-150">Owners have administrative privileges on the site so they can modify site pages and rebrand the site.</span></span> <span data-ttu-id="71eb1-151">他们还能够隐藏和显示通过 "学习路径" Web 部件传递的内容。</span><span class="sxs-lookup"><span data-stu-id="71eb1-151">They also have the ability to hide and show content delivered through the learning pathways Web part.</span></span> <span data-ttu-id="71eb1-152">此外, 他们还能够构建自定义播放列表并将其分配给自定义子类别。</span><span class="sxs-lookup"><span data-stu-id="71eb1-152">In addition, they'll have the ability to build custom playlist and assign them to custom subcategories.</span></span>  

1. <span data-ttu-id="71eb1-153">从 "SharePoint**设置**" 菜单中, 单击 "**网站权限**"。</span><span class="sxs-lookup"><span data-stu-id="71eb1-153">From the SharePoint **Settings** menu, click **Site Permissions**.</span></span>
2. <span data-ttu-id="71eb1-154">单击 "**高级权限设置**"。</span><span class="sxs-lookup"><span data-stu-id="71eb1-154">Click **Advanced Permission Settings**.</span></span>
3. <span data-ttu-id="71eb1-155">单击 " **Microsoft 365 学习路径所有者**"。</span><span class="sxs-lookup"><span data-stu-id="71eb1-155">Click **Microsoft 365 learning pathways Owners**.</span></span>
4. <span data-ttu-id="71eb1-156">单击 "**新建** > 向**此组添加用户**", 然后添加您希望成为所有者的人员。</span><span class="sxs-lookup"><span data-stu-id="71eb1-156">Click **New** > **Add Users to this group**, and then add the people you want to be Owners.</span></span> 
5. <span data-ttu-id="71eb1-157">添加链接以在共享邮件中[浏览网站](custom_exploresite.md), 然后单击 "**共享**"。</span><span class="sxs-lookup"><span data-stu-id="71eb1-157">Add a link to [Explore the Site](custom_exploresite.md) in the Share message, and then click **Share**.</span></span>

### <a name="next-steps"></a><span data-ttu-id="71eb1-158">后续步骤</span><span class="sxs-lookup"><span data-stu-id="71eb1-158">Next Steps</span></span>
- <span data-ttu-id="71eb1-159">浏览网站和 web 部件中提供的[默认内容](custom_exploresite.md)。</span><span class="sxs-lookup"><span data-stu-id="71eb1-159">Explore the [default content](custom_exploresite.md) provided in the site and web part.</span></span>
