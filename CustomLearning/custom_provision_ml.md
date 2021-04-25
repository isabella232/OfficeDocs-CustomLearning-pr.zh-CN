---
author: pkrebs
ms.author: pkrebs
title: 预配新的学习路径多语言解决方案
ms.date: 02/10/2019
description: 通过 SharePoint 预配服务预配 Microsoft 365 学习路径网站
ROBOTS: NOINDEX, NOFOLLOW
ms.service: sharepoint-online
manager: bpardi
ms.topic: article
audience: admin
ms.openlocfilehash: 40371138db2ec01e0e4a6558175f68cfa06fba51
ms.sourcegitcommit: 97e175e5ff5b6a9e0274d5ec9b39fdf7e18eb387
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/25/2021
ms.locfileid: "51999378"
---
# <a name="provision-a-new-learning-pathways-multilingual-solution"></a><span data-ttu-id="e9468-103">预配新的学习路径多语言解决方案</span><span class="sxs-lookup"><span data-stu-id="e9468-103">Provision a new learning pathways multilingual solution</span></span>
<span data-ttu-id="e9468-104">没有在租户中设置学习路径的组织可以使用 SharePoint 预配服务添加多语言学习路径解决方案。</span><span class="sxs-lookup"><span data-stu-id="e9468-104">Organizations that that don’t have learning pathways provisioned in their tenant can use the SharePoint Provisioning Service to add the multilingual learning pathways solution.</span></span> <span data-ttu-id="e9468-105">使用此选项，SharePoint 模板的学习路径将翻译为 9 种语言，并且可通过最少的修改来使用。</span><span class="sxs-lookup"><span data-stu-id="e9468-105">With this option, the learning pathways SharePoint template is translated into nine languages and can be used with a minimum of modification.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="e9468-106">如果你已在租户中预配了学习路径，建议你遵循更新 [路径学习路径](custom_update_ml.md) 。</span><span class="sxs-lookup"><span data-stu-id="e9468-106">If you already have learning pathways provisioned in your tenant, it's recommended that you follow the [update path](custom_update_ml.md) for learning pathways.</span></span> <span data-ttu-id="e9468-107">如果通过租户中的现有实例安装学习路径，则对学习路径网站模板或播放列表进行的任何更改都可能会丢失。</span><span class="sxs-lookup"><span data-stu-id="e9468-107">If you install learning pathways over an existing instance in your tenant, any changes made to the the learning pathways site template or playlists may be lost.</span></span>

## <a name="prerequisites-for-multilingual-support"></a><span data-ttu-id="e9468-108">多语言支持的先决条件</span><span class="sxs-lookup"><span data-stu-id="e9468-108">Prerequisites for multilingual support</span></span>
 
<span data-ttu-id="e9468-109">若要使用预配服务成功设置 Microsoft 365 学习路径，执行预配的人必须满足以下先决条件：</span><span class="sxs-lookup"><span data-stu-id="e9468-109">To successfully set up Microsoft 365 learning pathways with the Provisioning Service, the person doing the provisioning must meet the following pre-requisites:</span></span> 
 
- <span data-ttu-id="e9468-110">预配学习路径的人必须是将预配学习路径的租户的租户管理员。</span><span class="sxs-lookup"><span data-stu-id="e9468-110">The person provisioning learning pathways must be a Tenant Administrator of the tenant where learning pathways will be provisioned.</span></span>  
- <span data-ttu-id="e9468-111">租户应用程序目录必须在 SharePoint 管理中心的"应用程序"选项中提供。</span><span class="sxs-lookup"><span data-stu-id="e9468-111">A tenant App Catalog must be available within the Apps option of the SharePoint Admin Center.</span></span> <span data-ttu-id="e9468-112">如果您的组织没有 SharePoint 租户应用程序目录，请参阅 [SharePoint Online 文档以](/sharepoint/use-app-catalog) 创建一个。</span><span class="sxs-lookup"><span data-stu-id="e9468-112">If your organization doesn't have an SharePoint tenant App Catalog, refer to the [SharePoint Online documentation](/sharepoint/use-app-catalog) to create one.</span></span> <span data-ttu-id="e9468-113">在创建应用程序目录后，你必须等待至少两个小时，然后才能预配学习路径。</span><span class="sxs-lookup"><span data-stu-id="e9468-113">You must wait at least two hours after creating the App Catalog before provisioning learning pathways.</span></span>  
- <span data-ttu-id="e9468-114">预配学习路径的人必须是租户应用程序目录的网站集所有者。</span><span class="sxs-lookup"><span data-stu-id="e9468-114">The person provisioning learning pathways must be a Site Collection Owner of the Tenant App Catalog.</span></span> <span data-ttu-id="e9468-115">如果预配学习路径的人不是应用程序目录的网站集所有者，请 [完成这些](addappadmin.md) 说明并继续操作。</span><span class="sxs-lookup"><span data-stu-id="e9468-115">If the person provisioning learning pathways is not a Site Collection Owner of the App Catalog, [complete these instructions](addappadmin.md) and continue.</span></span> 

## <a name="ensure-the-tenant-admin-account-doesnt-have-a-language-selected"></a><span data-ttu-id="e9468-116">确保租户管理员帐户未选择语言</span><span class="sxs-lookup"><span data-stu-id="e9468-116">Ensure the Tenant Admin account doesn't have a language selected</span></span>
<span data-ttu-id="e9468-117">预配学习路径之前，请确保租户的管理员帐户未选择语言。</span><span class="sxs-lookup"><span data-stu-id="e9468-117">Before you provision learning pathways, ensure that the Admin Account for the tenant doesn't have a language selected.</span></span> <span data-ttu-id="e9468-118">下面将了解如何验证管理员帐户是否未选择语言。</span><span class="sxs-lookup"><span data-stu-id="e9468-118">Here’s how to verify if the Admin account doesn't have a language selected.</span></span> 
1.  <span data-ttu-id="e9468-119">使用边缘管理员配置文件，转到 office.com。</span><span class="sxs-lookup"><span data-stu-id="e9468-119">With your Edge Admin profile, go to office.com.</span></span>
2.  <span data-ttu-id="e9468-120">如有必要，请 (用户凭据) 。</span><span class="sxs-lookup"><span data-stu-id="e9468-120">Enter the user credentials (if necessary).</span></span>
3.  <span data-ttu-id="e9468-121">在 Microsoft 365 中，单击 **"Delve >** 应用"。</span><span class="sxs-lookup"><span data-stu-id="e9468-121">In Microsoft 365, click **All Apps** > Delve.</span></span> 
4.  <span data-ttu-id="e9468-122">单击 **"我**  >  **""更新配置文件"。**</span><span class="sxs-lookup"><span data-stu-id="e9468-122">Click **Me** > **Update Profile**.</span></span>
5.  <span data-ttu-id="e9468-123">向下滚动页面，然后单击 **如何更改语言和区域设置**。</span><span class="sxs-lookup"><span data-stu-id="e9468-123">Scroll down the page and click **How can I change language and regional settings**.</span></span>
6.  <span data-ttu-id="e9468-124">单击此处 **，** 然后单击省略号 **...。**</span><span class="sxs-lookup"><span data-stu-id="e9468-124">Click **here**, and then click the ellipses **...**.</span></span>
7.  <span data-ttu-id="e9468-125">在 **"我的显示语言**"下，应看到"**未选择任何语言"。**</span><span class="sxs-lookup"><span data-stu-id="e9468-125">Under **My Display Languages**, you should see **No languages selected**.</span></span> <span data-ttu-id="e9468-126">如果选择了语言，则取消选择该语言。</span><span class="sxs-lookup"><span data-stu-id="e9468-126">If a language is selected, unselect it.</span></span>

### <a name="to-provision-learning-pathways"></a><span data-ttu-id="e9468-127">设置学习路径</span><span class="sxs-lookup"><span data-stu-id="e9468-127">To provision learning pathways</span></span>

1. <span data-ttu-id="e9468-128">转到 [Microsoft 365 学习路径解决方案页面](https://provisioning.sharepointpnp.com/details/3df8bd55-b872-4c9d-88e3-6b2f05344239)。</span><span class="sxs-lookup"><span data-stu-id="e9468-128">Go to the [Microsoft 365 learning pathways solution page](https://provisioning.sharepointpnp.com/details/3df8bd55-b872-4c9d-88e3-6b2f05344239).</span></span>
2. <span data-ttu-id="e9468-129">单击 **"添加到你的租户"。**</span><span class="sxs-lookup"><span data-stu-id="e9468-129">Click **Add to your tenant**.</span></span> <span data-ttu-id="e9468-130">如果你未登录到租户，预配服务会要求你提供租户管理员凭据。</span><span class="sxs-lookup"><span data-stu-id="e9468-130">If you aren't signed into to your tenant, the Provisioning Service will ask for your Tenant Admin credentials.</span></span> 
3. <span data-ttu-id="e9468-131">在"请求的权限"对话框中，选择"代表你的组织同意 **"，** 然后选择"接受 **"。**</span><span class="sxs-lookup"><span data-stu-id="e9468-131">From the Permissions requested dialog box, select **Consent on behalf of your organization** and then select **Accept**.</span></span>

<span data-ttu-id="e9468-132">预配服务需要这些权限才能创建租户应用程序目录、将应用程序安装到租户应用程序目录并预配网站模板。</span><span class="sxs-lookup"><span data-stu-id="e9468-132">The provisioning service requires these permissions to create the tenant App Catalog, install the application into the tenant App Catalog and provision the site template.</span></span> <span data-ttu-id="e9468-133">对租户没有整体影响。</span><span class="sxs-lookup"><span data-stu-id="e9468-133">There's no overall impact on your tenant.</span></span> <span data-ttu-id="e9468-134">这些权限明确用于安装解决方案。</span><span class="sxs-lookup"><span data-stu-id="e9468-134">These permissions are explicitly used for the purpose of the solution installation.</span></span> <span data-ttu-id="e9468-135">必须接受这些权限才能继续安装。</span><span class="sxs-lookup"><span data-stu-id="e9468-135">You must accept these permissions to continue with the installation.</span></span>

4. <span data-ttu-id="e9468-136">根据需要填写预配信息页面上的字段。</span><span class="sxs-lookup"><span data-stu-id="e9468-136">Complete the fields on the provisioning information page as appropriate for your installation.</span></span> <span data-ttu-id="e9468-137">至少输入你希望接收预配流程相关通知的电子邮件地址，以及你要预配的网站的目标 URL。</span><span class="sxs-lookup"><span data-stu-id="e9468-137">At a minimum, enter the email address where you wish to get notifications about the provisioning process and the destination URL for your site to be provisioned to.</span></span>  
> [!NOTE]
> <span data-ttu-id="e9468-138">为你的员工提供合适的网站目标 URL，例如“/sites/MyTraining”或“/teams/LearnMicrosoft365”。</span><span class="sxs-lookup"><span data-stu-id="e9468-138">Make the destination URL for your site something friendly to your employees such as "/sites/MyTraining" or "/teams/LearnMicrosoft365".</span></span>

![inst_options.png](media/inst_options.png)

6. <span data-ttu-id="e9468-140">准备好 **将** 学习路径安装到租户环境中时，单击预配。</span><span class="sxs-lookup"><span data-stu-id="e9468-140">Click **Provision** when ready to install learning pathways into your tenant environment.</span></span>  <span data-ttu-id="e9468-141">预配流程最多可能需要 15 分钟。</span><span class="sxs-lookup"><span data-stu-id="e9468-141">The provisioning process can take up to 15 minutes.</span></span> <span data-ttu-id="e9468-142">网站准备就绪时，将通过电子邮件通知你。</span><span class="sxs-lookup"><span data-stu-id="e9468-142">You will be notified via email when the site is ready.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="e9468-143">设置学习路径网站的租户管理员必须转到该网站，然后打开 **CustomLearningAdmin.aspx** 以初始化学习路径管理员属性。</span><span class="sxs-lookup"><span data-stu-id="e9468-143">The Tenant Admin who provisions the learning pathways site must go to the site, and then open **CustomLearningAdmin.aspx** to initialize learning pathways Admin properties.</span></span> <span data-ttu-id="e9468-144">目前，租户管理员还应将所有者分配给网站。</span><span class="sxs-lookup"><span data-stu-id="e9468-144">At this time, the Tenant Admin should also assign Owners to the site.</span></span> 

## <a name="validate-provisioning-success-and-initialize-the-customconfig-list"></a><span data-ttu-id="e9468-145">验证预配成功并初始化 CustomConfig 列表</span><span class="sxs-lookup"><span data-stu-id="e9468-145">Validate Provisioning Success and Initialize the CustomConfig List</span></span>

<span data-ttu-id="e9468-146">预配完成后，预配网站的租户管理员将收到来自 PnP 预配服务的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="e9468-146">When provisioning is complete, the Tenant Admin who provisioned the site receives an email from the PnP Provisioning Service.</span></span> <span data-ttu-id="e9468-147">电子邮件包含指向网站的链接。</span><span class="sxs-lookup"><span data-stu-id="e9468-147">The email contains a link to the site.</span></span> <span data-ttu-id="e9468-148">此时，租户管理员应该使用电子邮件中提供的链接转到网站，并设置网站以首次使用：</span><span class="sxs-lookup"><span data-stu-id="e9468-148">At this point, the Tenant Admin should go to the site using the link provided in the email and set up the site for first use:</span></span>

- <span data-ttu-id="e9468-149">转到 `<YOUR-SITE-COLLECTION-URL>sites/<YOUR-SITE-NAME>/SitePages/CustomLearningAdmin.aspx`。</span><span class="sxs-lookup"><span data-stu-id="e9468-149">Go to `<YOUR-SITE-COLLECTION-URL>sites/<YOUR-SITE-NAME>/SitePages/CustomLearningAdmin.aspx`.</span></span> <span data-ttu-id="e9468-150">打开 **CustomLearningAdmin.aspx** 会初始化 **CustomConfig** 列表项，以设置首次使用的学习路径。</span><span class="sxs-lookup"><span data-stu-id="e9468-150">Opening **CustomLearningAdmin.aspx** initializes the **CustomConfig** list item that sets up learning pathways for first use.</span></span> <span data-ttu-id="e9468-151">应看到如下页面：</span><span class="sxs-lookup"><span data-stu-id="e9468-151">You should see a page that looks like this:</span></span>

![cg-adminapppage.png](media/cg-adminapppage.png)

## <a name="add-owners-to-site"></a><span data-ttu-id="e9468-153">将所有者添加到网站</span><span class="sxs-lookup"><span data-stu-id="e9468-153">Add Owners to Site</span></span>
<span data-ttu-id="e9468-154">作为租户管理员，你不太可能是自定义网站的人，因此你需要为网站分配几个所有者。</span><span class="sxs-lookup"><span data-stu-id="e9468-154">As the Tenant Admin, it's unlikely you'll be the person customizing the site, so you'll need to assign a few owners to the site.</span></span> <span data-ttu-id="e9468-155">所有者对网站拥有管理权限，因此可以修改网站页面和重新品牌。</span><span class="sxs-lookup"><span data-stu-id="e9468-155">Owners have administrative privileges on the site so they can modify site pages and rebrand the site.</span></span> <span data-ttu-id="e9468-156">他们还能够隐藏和显示内容，并生成自定义播放列表和子类别。</span><span class="sxs-lookup"><span data-stu-id="e9468-156">They also have the ability to hide and show content and build custom playlist and subcategories.</span></span>  

1. <span data-ttu-id="e9468-157">从"SharePoint **设置"菜单中**，单击"**网站权限"。**</span><span class="sxs-lookup"><span data-stu-id="e9468-157">From the SharePoint **Settings** menu, click **Site Permissions**.</span></span>
2. <span data-ttu-id="e9468-158">单击 **"高级权限设置"。**</span><span class="sxs-lookup"><span data-stu-id="e9468-158">Click **Advanced Permission Settings**.</span></span>
3. <span data-ttu-id="e9468-159">单击 **"Microsoft 365 学习路径所有者"。**</span><span class="sxs-lookup"><span data-stu-id="e9468-159">Click **Microsoft 365 learning pathways Owners**.</span></span>
4. <span data-ttu-id="e9468-160">单击 **"**  >  **新建向此组添加用户"，** 然后添加希望成为所有者的用户。</span><span class="sxs-lookup"><span data-stu-id="e9468-160">Click **New** > **Add Users to this group**, and then add the people you want to be Owners.</span></span> 
5. <span data-ttu-id="e9468-161">在"共享 ["消息中添加"浏览](custom_exploresite.md)网站"的链接，然后单击"共享 **"。**</span><span class="sxs-lookup"><span data-stu-id="e9468-161">Add a link to [Explore the Site](custom_exploresite.md) in the Share message, and then click **Share**.</span></span>

## <a name="add-translators-to-the-site"></a><span data-ttu-id="e9468-162">将翻译人员添加到网站</span><span class="sxs-lookup"><span data-stu-id="e9468-162">Add translators to the site</span></span>
<span data-ttu-id="e9468-163">如果要对网站使用翻译程序，可以为其分配权限。</span><span class="sxs-lookup"><span data-stu-id="e9468-163">If you will be using translators for the site, you can assign them permissions.</span></span> <span data-ttu-id="e9468-164">翻译人员需要成员权限或更高权限。</span><span class="sxs-lookup"><span data-stu-id="e9468-164">Translators require Member permissions or higher.</span></span> 

## <a name="choose-options-for-using-multiple-languages-on-the-site"></a><span data-ttu-id="e9468-165">选择用于网站上多种语言的选项</span><span class="sxs-lookup"><span data-stu-id="e9468-165">Choose options for using multiple languages on the site</span></span>
<span data-ttu-id="e9468-166">SharePoint 设置服务使用九种语言创建学习路径网站。</span><span class="sxs-lookup"><span data-stu-id="e9468-166">The SharePoint Provisioning Service creates the Learning Pathways site in nine languages.</span></span> <span data-ttu-id="e9468-167">以下建议适用：</span><span class="sxs-lookup"><span data-stu-id="e9468-167">The following recommendations apply:</span></span>
- <span data-ttu-id="e9468-168">关闭不希望支持的语言</span><span class="sxs-lookup"><span data-stu-id="e9468-168">Turn off the languages you don’t want to support</span></span>
- <span data-ttu-id="e9468-169">如果您不支持多语言网站，请关闭多语言功能。</span><span class="sxs-lookup"><span data-stu-id="e9468-169">If you are not supporting a multilingual site, turn off the multi-lingual feature.</span></span> <span data-ttu-id="e9468-170">请参阅本主题稍后的"关闭多语言支持"部分。</span><span class="sxs-lookup"><span data-stu-id="e9468-170">See the "Turn off multilingual support" section later in this topic.</span></span>

### <a name="remove-languages-you-dont-want-to-support"></a><span data-ttu-id="e9468-171">删除不希望支持的语言</span><span class="sxs-lookup"><span data-stu-id="e9468-171">Remove languages you don’t want to support</span></span>
<span data-ttu-id="e9468-172">对于选择仅支持一种语言（除了默认英语语言）的组织，我们建议删除不支持的语言。</span><span class="sxs-lookup"><span data-stu-id="e9468-172">For organizations that choose to support only one language, in addition to the default English language, we recommend removing languages that aren’t supported.</span></span> 
1. <span data-ttu-id="e9468-173">从"学习路径"网站中，从页面的右上方选择"设置"，然后选择"网站 **信息"。**</span><span class="sxs-lookup"><span data-stu-id="e9468-173">From the Learning Pathways site, select **Settings** from the top-right of the page, and then select **Site information**.</span></span>
2. <span data-ttu-id="e9468-174">在网站信息窗格底部，选择"**查看所有网站设置"。**</span><span class="sxs-lookup"><span data-stu-id="e9468-174">At the bottom of the site information pane, select **View all site settings**.</span></span>
3. <span data-ttu-id="e9468-175">在 **"网站管理"下**，选择"**语言设置"。**</span><span class="sxs-lookup"><span data-stu-id="e9468-175">Under **Site Administration**, select **Language settings**.</span></span>
4. <span data-ttu-id="e9468-176">在 **"启用要翻译为多种语言的页面** 和新闻"下，将开关滑动到 **"打开"。**</span><span class="sxs-lookup"><span data-stu-id="e9468-176">Under **Enable pages and news to be translated into multiple languages**, slide the toggle to **On**.</span></span> <span data-ttu-id="e9468-177">默认情况下应为"打开"。</span><span class="sxs-lookup"><span data-stu-id="e9468-177">It should be On by default.</span></span>
5. <span data-ttu-id="e9468-178">在"添加或删除网站语言"下，单击"删除"以删除网站不需要的语言。</span><span class="sxs-lookup"><span data-stu-id="e9468-178">Under Add or remove site languages, click **Remove** to remove the languages you don't need for the site.</span></span> <span data-ttu-id="e9468-179">下面显示了"语言设置"页的示例，除了显示默认英语语言之外，还显示网站支持的意大利语。</span><span class="sxs-lookup"><span data-stu-id="e9468-179">The following shows an example of the Language Settings page to show Italian supported for the site, in addition to the default English language.</span></span>

![custom_update_ml_langsettings.png](media/custom_update_ml_langsettings.png)

> [!NOTE]
> <span data-ttu-id="e9468-181">删除语言时，不能删除默认的英语语言。</span><span class="sxs-lookup"><span data-stu-id="e9468-181">When removing languages you cannot remove the default English language.</span></span> 

### <a name="assign-translators"></a><span data-ttu-id="e9468-182">分配翻译人员</span><span class="sxs-lookup"><span data-stu-id="e9468-182">Assign translators</span></span>
<span data-ttu-id="e9468-183">如果要翻译页面，可选择为每个语言分配一个或多个翻译 (网站默认语言除外) 。</span><span class="sxs-lookup"><span data-stu-id="e9468-183">If you're going to translate pages, optionally assign one or more translators for each language (except the site default language).</span></span> 
- <span data-ttu-id="e9468-184">在 **"转换器** "列中，开始键入要成为翻译人员的人的名称，然后从列表中选择该姓名。</span><span class="sxs-lookup"><span data-stu-id="e9468-184">In the **Translator** column, start typing the name of a person you want to be a translator, and then select the name from the list.</span></span> 

> [!NOTE]
> <span data-ttu-id="e9468-185">可以将您组织的 Active Directory 中的任何人分配为翻译人员。</span><span class="sxs-lookup"><span data-stu-id="e9468-185">Anyone in your organization's Active Directory can be assigned as a translator.</span></span> <span data-ttu-id="e9468-186">不会自动为被分配为翻译人员的用户授予适当的权限。</span><span class="sxs-lookup"><span data-stu-id="e9468-186">People assigned as translators will not automatically be given appropriate permissions.</span></span> <span data-ttu-id="e9468-187">当没有网站编辑权限的用户尝试访问该网站时，他们将被定向到可以请求访问的网页。</span><span class="sxs-lookup"><span data-stu-id="e9468-187">When someone without edit permissions to a site tries to access the site, they will be directed to a web page where they can request access.</span></span>

## <a name="turn-off-multilingual-support"></a><span data-ttu-id="e9468-188">关闭多语言支持</span><span class="sxs-lookup"><span data-stu-id="e9468-188">Turn off multilingual support</span></span>
<span data-ttu-id="e9468-189">例如，如果您不需要多语言网站，您需要一个仅英文网站，建议您关闭多语言功能。</span><span class="sxs-lookup"><span data-stu-id="e9468-189">If you don’t want a multilingual site, for example, you want an English-only site, it’s recommended that you turn off the multilingual feature.</span></span> 

1. <span data-ttu-id="e9468-190">从"学习路径"网站中，从页面的右上方选择"设置"，然后选择"网站 **信息"。**</span><span class="sxs-lookup"><span data-stu-id="e9468-190">From the Learning Pathways site, select **Settings** from the top-right of the page, and then select **Site information**.</span></span>
2. <span data-ttu-id="e9468-191">在网站信息窗格底部，选择"**查看所有网站设置"。**</span><span class="sxs-lookup"><span data-stu-id="e9468-191">At the bottom of the site information pane, select **View all site settings**.</span></span>
3. <span data-ttu-id="e9468-192">在 **"网站管理"下**，选择"**语言设置"。**</span><span class="sxs-lookup"><span data-stu-id="e9468-192">Under **Site Administration**, select **Language settings**.</span></span>
4. <span data-ttu-id="e9468-193">在 **"启用要翻译为多种语言的页面** 和新闻"下，将开关滑动到 **"打开"。**</span><span class="sxs-lookup"><span data-stu-id="e9468-193">Under **Enable pages and news to be translated into multiple languages**, slide the toggle to **On**.</span></span> <span data-ttu-id="e9468-194">默认情况下应为"打开"。</span><span class="sxs-lookup"><span data-stu-id="e9468-194">It should be On by default.</span></span>
- <span data-ttu-id="e9468-195">在 **"启用要翻译的页面和新闻"下，** 选择"**关闭"。**</span><span class="sxs-lookup"><span data-stu-id="e9468-195">Under **Enable pages and news to be translated**, select **Off**.</span></span> 

### <a name="add-languages"></a><span data-ttu-id="e9468-196">添加语言</span><span class="sxs-lookup"><span data-stu-id="e9468-196">Add languages</span></span>
<span data-ttu-id="e9468-197">学习路径支持 9 种语言，但建议仅添加学习路径网站所需的语言。</span><span class="sxs-lookup"><span data-stu-id="e9468-197">Learning pathways supports 9 languages, but it’s recommended that you add only the languages you need to support for the learning pathways site.</span></span> <span data-ttu-id="e9468-198">你随时都可以添加语言。</span><span class="sxs-lookup"><span data-stu-id="e9468-198">You can add langauges at any time.</span></span> 
- <span data-ttu-id="e9468-199">在 **"添加或删除网站语言"下**，开始在"选择或键入语言"中键入语言名称，或者从下拉列表中选择语言。</span><span class="sxs-lookup"><span data-stu-id="e9468-199">Under **Add or remove site languages**, start typing a language name in **Select or type a language**, or choose a language from the dropdown.</span></span> <span data-ttu-id="e9468-200">可以重复此步骤以添加多种语言。</span><span class="sxs-lookup"><span data-stu-id="e9468-200">You can repeat this step to add multiple languages.</span></span> <span data-ttu-id="e9468-201">通过返回到此页面，您随时都可以在网站中添加或删除语言。</span><span class="sxs-lookup"><span data-stu-id="e9468-201">You can add or remove languages from your site at any time by going back to this page.</span></span>