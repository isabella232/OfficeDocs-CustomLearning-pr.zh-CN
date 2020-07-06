---
author: pkrebs
ms.author: pkrebs
title: 设置新的学习路径多语言解决方案
ms.date: 02/10/2019
description: 通过 SharePoint 设置服务设置 Microsoft 365 学习路径网站
ROBOTS: NOINDEX, NOFOLLOW
ms.openlocfilehash: 6948162d8a96c9a6582484c5f4fc8acad18405a7
ms.sourcegitcommit: f355885fb93d66abf61df535fa704ccdb8df9b64
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/05/2020
ms.locfileid: "45038992"
---
# <a name="provision-a-new-learning-pathways-multilingual-solution"></a><span data-ttu-id="ac9d0-103">设置新的学习路径多语言解决方案</span><span class="sxs-lookup"><span data-stu-id="ac9d0-103">Provision a new learning pathways multilingual solution</span></span>
<span data-ttu-id="ac9d0-104">如果组织没有在其租户中预配的学习路径，则可以使用 SharePoint 设置服务添加多语言学习路径解决方案。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-104">Organizations that that don’t have learning pathways provisioned in their tenant can use the SharePoint Provisioning Service to add the multilingual learning pathways solution.</span></span> <span data-ttu-id="ac9d0-105">使用此选项，可将 "学习路径" SharePoint 模板转换为九种语言，并且可以使用至少修改。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-105">With this option, the learning pathways SharePoint template is translated into nine languages and can be used with a minimum of modification.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="ac9d0-106">如果你已在租户中预配了学习路径，建议你遵循学习路径的[更新路径](custom_update_ml.md)。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-106">If you already have learning pathways provisioned in your tenant, it's recommended that you follow the [update path](custom_update_ml.md) for learning pathways.</span></span> <span data-ttu-id="ac9d0-107">如果您在租户中通过现有实例安装学习路径，则对 "学习路径" 网站模板或播放列表所做的任何更改都将丢失。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-107">If you install learning pathways over an existing instance in your tenant, any changes made to the the learning pathways site template or playlists may be lost.</span></span>

## <a name="prerequisites-for-multilingual-support"></a><span data-ttu-id="ac9d0-108">多语言支持的先决条件</span><span class="sxs-lookup"><span data-stu-id="ac9d0-108">Prerequisites for multilingual support</span></span>
 
<span data-ttu-id="ac9d0-109">若要成功设置与预配服务的 Microsoft 365 学习路径，执行预配的人员必须满足以下先决条件：</span><span class="sxs-lookup"><span data-stu-id="ac9d0-109">To successfully set up Microsoft 365 learning pathways with the Provisioning Service, the person doing the provisioning must meet the following pre-requisites:</span></span> 
 
- <span data-ttu-id="ac9d0-110">人员预配学习路径必须是租户的租户管理员，其中将预配学习路径。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-110">The person provisioning learning pathways must be a Tenant Administrator of the tenant where learning pathways will be provisioned.</span></span>  
- <span data-ttu-id="ac9d0-111">租户应用程序目录必须在 SharePoint 管理中心的 "应用程序" 选项中可用。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-111">A tenant App Catalog must be available within the Apps option of the SharePoint Admin Center.</span></span> <span data-ttu-id="ac9d0-112">如果您的组织没有 SharePoint 租户应用程序目录，请参阅[SharePoint Online 文档](https://docs.microsoft.com/sharepoint/use-app-catalog)以创建一个。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-112">If your organization doesn't have an SharePoint tenant App Catalog, refer to the [SharePoint Online documentation](https://docs.microsoft.com/sharepoint/use-app-catalog) to create one.</span></span> <span data-ttu-id="ac9d0-113">在设置学习路径之前，创建应用程序目录后，必须等待至少两小时。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-113">You must wait at least two hours after creating the App Catalog before provisioning learning pathways.</span></span>  
- <span data-ttu-id="ac9d0-114">人员预配学习路径必须是租户应用程序目录的网站集所有者。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-114">The person provisioning learning pathways must be a Site Collection Owner of the Tenant App Catalog.</span></span> <span data-ttu-id="ac9d0-115">如果人员设置学习路径不是应用程序目录的网站集所有者，请[完成这些说明](addappadmin.md)并继续。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-115">If the person provisioning learning pathways is not a Site Collection Owner of the App Catalog, [complete these instructions](addappadmin.md) and continue.</span></span> 

## <a name="ensure-the-tenant-admin-account-doesnt-have-a-language-selected"></a><span data-ttu-id="ac9d0-116">确保租户管理员帐户未选择所需的语言</span><span class="sxs-lookup"><span data-stu-id="ac9d0-116">Ensure the Tenant Admin account doesn't have a language selected</span></span>
<span data-ttu-id="ac9d0-117">在设置学习路径之前，请确保租户的管理员帐户没有选定的语言。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-117">Before you provision learning pathways, ensure that the Admin Account for the tenant doesn't have a language selected.</span></span> <span data-ttu-id="ac9d0-118">下面介绍如何验证管理员帐户是否未选择所需的语言。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-118">Here’s how to verify if the Admin account doesn't have a language selected.</span></span> 
1.  <span data-ttu-id="ac9d0-119">在边缘管理配置文件中，转到 "office.com"。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-119">With your Edge Admin profile, go to office.com.</span></span>
2.  <span data-ttu-id="ac9d0-120">输入用户凭据（如有必要）。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-120">Enter the user credentials (if necessary).</span></span>
3.  <span data-ttu-id="ac9d0-121">在 Microsoft 365 中，单击 "**所有应用**" > Delve。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-121">In Microsoft 365, click **All Apps** > Delve.</span></span> 
4.  <span data-ttu-id="ac9d0-122">单击 **"**  >  **更新配置文件**"。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-122">Click **Me** > **Update Profile**.</span></span>
5.  <span data-ttu-id="ac9d0-123">向下滚动页面并单击**如何更改语言和区域设置**。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-123">Scroll down the page and click **How can I change language and regional settings**.</span></span>
6.  <span data-ttu-id="ac9d0-124">单击**此处**，然后单击省略号 **...**。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-124">Click **here**, and then click the ellipses **...**.</span></span>
7.  <span data-ttu-id="ac9d0-125">在 **"我的显示语言**" 下，您应该会看到**未选中任何语言**。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-125">Under **My Display Languages**, you should see **No languages selected**.</span></span> <span data-ttu-id="ac9d0-126">如果选择了语言，请取消选择该语言。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-126">If a language is selected, unselect it.</span></span>

### <a name="to-provision-learning-pathways"></a><span data-ttu-id="ac9d0-127">设置学习路径</span><span class="sxs-lookup"><span data-stu-id="ac9d0-127">To provision learning pathways</span></span>

1. <span data-ttu-id="ac9d0-128">转到 " [Microsoft 365 学习路径解决方案" 页面](https://provisioning.sharepointpnp.com/details/3df8bd55-b872-4c9d-88e3-6b2f05344239)。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-128">Go to the [Microsoft 365 learning pathways solution page](https://provisioning.sharepointpnp.com/details/3df8bd55-b872-4c9d-88e3-6b2f05344239).</span></span>
2. <span data-ttu-id="ac9d0-129">单击 "**添加到你的租户**"。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-129">Click **Add to your tenant**.</span></span> <span data-ttu-id="ac9d0-130">如果你未登录到你的租户，设置服务将要求你提供租户管理员凭据。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-130">If you aren't signed into to your tenant, the Provisioning Service will ask for your Tenant Admin credentials.</span></span> 
3. <span data-ttu-id="ac9d0-131">从 "请求的权限" 对话框中，选择**代表你的组织同意**的，然后选择 "**接受**"。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-131">From the Permissions requested dialog box, select **Consent on behalf of your organization** and then select **Accept**.</span></span>

<span data-ttu-id="ac9d0-132">预配服务需要这些权限才能创建租户应用程序目录，请将应用程序安装到租户应用目录中并预配网站模板。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-132">The provisioning service requires these permissions to create the tenant App Catalog, install the application into the tenant App Catalog and provision the site template.</span></span> <span data-ttu-id="ac9d0-133">对租户没有整体影响。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-133">There's no overall impact on your tenant.</span></span> <span data-ttu-id="ac9d0-134">这些权限将显式用于解决方案安装的目的。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-134">These permissions are explicitly used for the purpose of the solution installation.</span></span> <span data-ttu-id="ac9d0-135">您必须接受这些权限才能继续安装。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-135">You must accept these permissions to continue with the installation.</span></span>

4. <span data-ttu-id="ac9d0-136">根据您的安装需要填写 "设置信息" 页上的字段。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-136">Complete the fields on the provisioning information page as appropriate for your installation.</span></span> <span data-ttu-id="ac9d0-137">请至少输入你希望获取有关设置过程的通知的电子邮件地址和要设置为的网站的目标 URL。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-137">At a minimum, enter the email address where you wish to get notifications about the provisioning process and the destination URL for your site to be provisioned to.</span></span>  
> [!NOTE]
> <span data-ttu-id="ac9d0-138">将网站的目标 URL 设置为友好的内容，如 "/sites/MyTraining" 或 "/teams/LearnMicrosoft365"。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-138">Make the destination URL for your site something friendly to your employees such as "/sites/MyTraining" or "/teams/LearnMicrosoft365".</span></span>

![inst_options.png](media/inst_options.png)

6. <span data-ttu-id="ac9d0-140">准备好将学习路径安装到你的租户环境中时，请单击 "**设置**"。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-140">Click **Provision** when ready to install learning pathways into your tenant environment.</span></span>  <span data-ttu-id="ac9d0-141">预配过程最长可能需要15分钟。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-141">The provisioning process can take up to 15 minutes.</span></span> <span data-ttu-id="ac9d0-142">当网站准备就绪时，将通过电子邮件通知你。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-142">You will be notified via email when the site is ready.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="ac9d0-143">预配学习路径网站的租户管理员必须转到网站，然后打开**CustomLearningAdmin**以初始化 "学习路径管理" 属性。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-143">The Tenant Admin who provisions the learning pathways site must go to the site, and then open **CustomLearningAdmin.aspx** to initialize learning pathways Admin properties.</span></span> <span data-ttu-id="ac9d0-144">目前，租户管理员还应将所有者分配给网站。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-144">At this time, the Tenant Admin should also assign Owners to the site.</span></span> 

## <a name="validate-provisioning-success-and-initialize-the-customconfig-list"></a><span data-ttu-id="ac9d0-145">验证设置是否成功并初始化 CustomConfig 列表</span><span class="sxs-lookup"><span data-stu-id="ac9d0-145">Validate Provisioning Success and Initialize the CustomConfig List</span></span>

<span data-ttu-id="ac9d0-146">设置完成后，预配网站的租户管理员将收到来自 PnP 预配服务的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-146">When provisioning is complete, the Tenant Admin who provisioned the site receives an email from the PnP Provisioning Service.</span></span> <span data-ttu-id="ac9d0-147">电子邮件包含指向该网站的链接。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-147">The email contains a link to the site.</span></span> <span data-ttu-id="ac9d0-148">在这种情况下，租户管理员应使用电子邮件中提供的链接转到网站，并将网站设置为首次使用：</span><span class="sxs-lookup"><span data-stu-id="ac9d0-148">At this point, the Tenant Admin should go to the site using the link provided in the email and set up the site for first use:</span></span>

- <span data-ttu-id="ac9d0-149">转到 `<YOUR-SITE-COLLECTION-URL>sites/<YOUR-SITE-NAME>/SitePages/CustomLearningAdmin.aspx`。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-149">Go to `<YOUR-SITE-COLLECTION-URL>sites/<YOUR-SITE-NAME>/SitePages/CustomLearningAdmin.aspx`.</span></span> <span data-ttu-id="ac9d0-150">打开**CustomLearningAdmin**可初始化**CustomConfig**列表项，该列表项设置首次使用的学习路径。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-150">Opening **CustomLearningAdmin.aspx** initializes the **CustomConfig** list item that sets up learning pathways for first use.</span></span> <span data-ttu-id="ac9d0-151">您应该会看到如下所示的页面：</span><span class="sxs-lookup"><span data-stu-id="ac9d0-151">You should see a page that looks like this:</span></span>

![cg-adminapppage.png](media/cg-adminapppage.png)

## <a name="add-owners-to-site"></a><span data-ttu-id="ac9d0-153">将所有者添加到网站</span><span class="sxs-lookup"><span data-stu-id="ac9d0-153">Add Owners to Site</span></span>
<span data-ttu-id="ac9d0-154">作为租户管理员，您不太可能是自定义网站的人员，因此您需要向网站分配一些所有者。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-154">As the Tenant Admin, it's unlikely you'll be the person customizing the site, so you'll need to assign a few owners to the site.</span></span> <span data-ttu-id="ac9d0-155">所有者具有对网站的管理权限，以便他们可以修改网站页面并 rebrand 网站。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-155">Owners have administrative privileges on the site so they can modify site pages and rebrand the site.</span></span> <span data-ttu-id="ac9d0-156">他们还能够隐藏和显示内容，并生成自定义的播放列表和子类别。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-156">They also have the ability to hide and show content and build custom playlist and subcategories.</span></span>  

1. <span data-ttu-id="ac9d0-157">从 "SharePoint**设置**" 菜单中，单击 "**网站权限**"。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-157">From the SharePoint **Settings** menu, click **Site Permissions**.</span></span>
2. <span data-ttu-id="ac9d0-158">单击 "**高级权限设置**"。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-158">Click **Advanced Permission Settings**.</span></span>
3. <span data-ttu-id="ac9d0-159">单击 " **Microsoft 365 学习路径所有者**"。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-159">Click **Microsoft 365 learning pathways Owners**.</span></span>
4. <span data-ttu-id="ac9d0-160">单击 "**新建**向  >  **此组添加用户**"，然后添加您希望成为所有者的人员。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-160">Click **New** > **Add Users to this group**, and then add the people you want to be Owners.</span></span> 
5. <span data-ttu-id="ac9d0-161">添加链接以在共享邮件中[浏览网站](custom_exploresite.md)，然后单击 "**共享**"。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-161">Add a link to [Explore the Site](custom_exploresite.md) in the Share message, and then click **Share**.</span></span>

## <a name="add-translators-to-the-site"></a><span data-ttu-id="ac9d0-162">将翻译者添加到网站</span><span class="sxs-lookup"><span data-stu-id="ac9d0-162">Add translators to the site</span></span>
<span data-ttu-id="ac9d0-163">如果要使用网站的翻译人员，可以为其分配权限。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-163">If you will be using translators for the site, you can assign them permissions.</span></span> <span data-ttu-id="ac9d0-164">翻译人员需要成员权限或更高版本。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-164">Translators require Member permissions or higher.</span></span> 

## <a name="choose-options-for-using-multiple-languages-on-the-site"></a><span data-ttu-id="ac9d0-165">选择用于在网站上使用多种语言的选项</span><span class="sxs-lookup"><span data-stu-id="ac9d0-165">Choose options for using multiple languages on the site</span></span>
<span data-ttu-id="ac9d0-166">SharePoint 设置服务创建了九种语言的学习路径网站。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-166">The SharePoint Provisioning Service creates the Learning Pathways site in nine languages.</span></span> <span data-ttu-id="ac9d0-167">以下建议适用：</span><span class="sxs-lookup"><span data-stu-id="ac9d0-167">The following recommendations apply:</span></span>
- <span data-ttu-id="ac9d0-168">关闭不希望支持的语言</span><span class="sxs-lookup"><span data-stu-id="ac9d0-168">Turn off the languages you don’t want to support</span></span>
- <span data-ttu-id="ac9d0-169">如果不支持多语言网站，请关闭多语言功能。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-169">If you are not supporting a multilingual site, turn off the multi-lingual feature.</span></span> <span data-ttu-id="ac9d0-170">请参阅本主题后面的 "关闭多语言支持" 部分。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-170">See the "Turn off multilingual support" section later in this topic.</span></span>

### <a name="remove-languages-you-dont-want-to-support"></a><span data-ttu-id="ac9d0-171">删除不希望支持的语言</span><span class="sxs-lookup"><span data-stu-id="ac9d0-171">Remove languages you don’t want to support</span></span>
<span data-ttu-id="ac9d0-172">对于选择仅支持一种语言的组织，除了默认的英语语言外，我们建议删除不受支持的语言。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-172">For organizations that choose to support only one language, in addition to the default English language, we recommend removing languages that aren’t supported.</span></span> 
1. <span data-ttu-id="ac9d0-173">从 "学习路径" 网站中，从页面的右上方选择 "**设置**"，然后选择 "**网站信息**"。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-173">From the Learning Pathways site, select **Settings** from the top-right of the page, and then select **Site information**.</span></span>
2. <span data-ttu-id="ac9d0-174">在 "网站信息" 窗格的底部，选择 "**查看所有网站设置**"。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-174">At the bottom of the site information pane, select **View all site settings**.</span></span>
3. <span data-ttu-id="ac9d0-175">在 "**网站管理**" 下，选择 "**语言设置**"。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-175">Under **Site Administration**, select **Language settings**.</span></span>
4. <span data-ttu-id="ac9d0-176">在 "**允许将页面和新闻转换为多种语言**" 下，将切换滑到 **"打开**"。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-176">Under **Enable pages and news to be translated into multiple languages**, slide the toggle to **On**.</span></span> <span data-ttu-id="ac9d0-177">默认情况下，它应处于打开状态。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-177">It should be On by default.</span></span>
5. <span data-ttu-id="ac9d0-178">在 "添加或删除网站语言" 下，单击 "**删除**" 以删除网站不需要的语言。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-178">Under Add or remove site languages, click **Remove** to remove the languages you don't need for the site.</span></span> <span data-ttu-id="ac9d0-179">下面显示了 "语言设置" 页的一个示例，用于显示网站支持的意大利语，以及默认的英语语言。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-179">The following shows an example of the Language Settings page to show Italian supported for the site, in addition to the default English language.</span></span>

![custom_update_ml_langsettings.png](media/custom_update_ml_langsettings.png)

> [!NOTE]
> <span data-ttu-id="ac9d0-181">删除语言时，不能删除默认的英语语言。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-181">When removing languages you cannot remove the default English language.</span></span> 

### <a name="assign-translators"></a><span data-ttu-id="ac9d0-182">分配翻译人员</span><span class="sxs-lookup"><span data-stu-id="ac9d0-182">Assign translators</span></span>
<span data-ttu-id="ac9d0-183">如果要翻译页面，可以选择为每种语言分配一个或多个翻译人员（网站默认语言除外）。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-183">If you're going to translate pages, optionally assign one or more translators for each language (except the site default language).</span></span> 
- <span data-ttu-id="ac9d0-184">在 "**转换器**" 列中，开始键入要成为翻译人员的人员的姓名，然后从列表中选择名称。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-184">In the **Translator** column, start typing the name of a person you want to be a translator, and then select the name from the list.</span></span> 

> [!NOTE]
> <span data-ttu-id="ac9d0-185">您组织的 Active Directory 中的任何人都可以作为翻译者进行分配。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-185">Anyone in your organization's Active Directory can be assigned as a translator.</span></span> <span data-ttu-id="ac9d0-186">被分配为翻译者的人员不会被自动授予适当的权限。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-186">People assigned as translators will not automatically be given appropriate permissions.</span></span> <span data-ttu-id="ac9d0-187">如果没有网站的 "编辑" 权限的用户尝试访问该网站，则会将其定向到可请求访问的网页。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-187">When someone without edit permissions to a site tries to access the site, they will be directed to a web page where they can request access.</span></span>

## <a name="turn-off-multilingual-support"></a><span data-ttu-id="ac9d0-188">关闭多语言支持</span><span class="sxs-lookup"><span data-stu-id="ac9d0-188">Turn off multilingual support</span></span>
<span data-ttu-id="ac9d0-189">例如，如果您不希望使用多语言网站，则建议您关闭多语言的网站。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-189">If you don’t want a multilingual site, for example, you want an English-only site, it’s recommended that you turn off the multilingual feature.</span></span> 

1. <span data-ttu-id="ac9d0-190">从 "学习路径" 网站中，从页面的右上方选择 "**设置**"，然后选择 "**网站信息**"。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-190">From the Learning Pathways site, select **Settings** from the top-right of the page, and then select **Site information**.</span></span>
2. <span data-ttu-id="ac9d0-191">在 "网站信息" 窗格的底部，选择 "**查看所有网站设置**"。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-191">At the bottom of the site information pane, select **View all site settings**.</span></span>
3. <span data-ttu-id="ac9d0-192">在 "**网站管理**" 下，选择 "**语言设置**"。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-192">Under **Site Administration**, select **Language settings**.</span></span>
4. <span data-ttu-id="ac9d0-193">在 "**允许将页面和新闻转换为多种语言**" 下，将切换滑到 **"打开**"。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-193">Under **Enable pages and news to be translated into multiple languages**, slide the toggle to **On**.</span></span> <span data-ttu-id="ac9d0-194">默认情况下，它应处于打开状态。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-194">It should be On by default.</span></span>
- <span data-ttu-id="ac9d0-195">在 "**启用要翻译的页面和新闻**" 下，选择 "**关闭**"。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-195">Under **Enable pages and news to be translated**, select **Off**.</span></span> 

### <a name="add-languages"></a><span data-ttu-id="ac9d0-196">添加语言</span><span class="sxs-lookup"><span data-stu-id="ac9d0-196">Add languages</span></span>
<span data-ttu-id="ac9d0-197">学习路径支持9种语言，但建议您仅添加支持学习路径网站所需的语言。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-197">Learning pathways supports 9 languages, but it’s recommended that you add only the languages you need to support for the learning pathways site.</span></span> <span data-ttu-id="ac9d0-198">您可以随时添加语言。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-198">You can add langauges at any time.</span></span> 
- <span data-ttu-id="ac9d0-199">在 "**添加或删除网站语言**" 下，开始在 "**选择" 或 "键入语言**" 中键入语言名称，或从下拉列表中选择一种语言。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-199">Under **Add or remove site languages**, start typing a language name in **Select or type a language**, or choose a language from the dropdown.</span></span> <span data-ttu-id="ac9d0-200">您可以重复此步骤以添加多种语言。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-200">You can repeat this step to add multiple languages.</span></span> <span data-ttu-id="ac9d0-201">您可以通过返回到此页随时在网站中添加或删除语言。</span><span class="sxs-lookup"><span data-stu-id="ac9d0-201">You can add or remove languages from your site at any time by going back to this page.</span></span>



