---
author: pkrebs
ms.author: pkrebs
title: 更新多语言支持的学习路径
ms.date: 05/20/2019
description: 更新多语言支持的学习路径
ROBOTS: NOINDEX, NOFOLLOW
ms.service: sharepoint-online
manager: bpardi
ms.topic: article
audience: admin
ms.openlocfilehash: 9344cd91e5b6718b1eb0e73e25fdc8311afed793
ms.sourcegitcommit: 97e175e5ff5b6a9e0274d5ec9b39fdf7e18eb387
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/25/2021
ms.locfileid: "52000238"
---
# <a name="update-learning-pathways-for-multilingual-support"></a><span data-ttu-id="0c2ad-103">更新多语言支持的学习路径</span><span class="sxs-lookup"><span data-stu-id="0c2ad-103">Update learning pathways for multilingual support</span></span>
<span data-ttu-id="0c2ad-104">如果你有一个现有的学习路径网站，你可以更新它，实现多语言支持。</span><span class="sxs-lookup"><span data-stu-id="0c2ad-104">If you have an existing Learning Pathways site, you can update it for multilingual support.</span></span> <span data-ttu-id="0c2ad-105">若要更新多语言 4.0 版本的学习路径，需要将 Web 部件包 customlearning.sppkg 上载到 SharePoint 租户应用程序目录。</span><span class="sxs-lookup"><span data-stu-id="0c2ad-105">To update learning pathways to the multilingual 4.0 version, you upload the web part package, customlearning.sppkg, to the SharePoint tenant App Catalog.</span></span> <span data-ttu-id="0c2ad-106">更新学习路径时：</span><span class="sxs-lookup"><span data-stu-id="0c2ad-106">When you update learning pathways:</span></span>  

- <span data-ttu-id="0c2ad-107">保留以前创建的任何自定义播放列表和资产</span><span class="sxs-lookup"><span data-stu-id="0c2ad-107">Any previously created custom playlists and assets are maintained</span></span>
- <span data-ttu-id="0c2ad-108">用于隐藏或显示内容的设置将保留</span><span class="sxs-lookup"><span data-stu-id="0c2ad-108">Settings to hide or show content are maintained</span></span>
- <span data-ttu-id="0c2ad-109">SharePoint 模板的学习路径保持不变</span><span class="sxs-lookup"><span data-stu-id="0c2ad-109">The learning pathways SharePoint template is left unchanged</span></span>
- <span data-ttu-id="0c2ad-110">不会翻译学习路径网站页面。</span><span class="sxs-lookup"><span data-stu-id="0c2ad-110">The learning pathways site pages aren't translated.</span></span> <span data-ttu-id="0c2ad-111">必须手动完成此工作</span><span class="sxs-lookup"><span data-stu-id="0c2ad-111">This work must be done manually</span></span>

## <a name="read-the-learning-pathways-multilingual-overview"></a><span data-ttu-id="0c2ad-112">阅读学习路径多语言概述</span><span class="sxs-lookup"><span data-stu-id="0c2ad-112">Read the learning pathways multilingual overview</span></span>
<span data-ttu-id="0c2ad-113">若要了解多语言支持如何用于学习路径，请阅读学习路径 [多语言概述](custom_overview_ml.md)) 。</span><span class="sxs-lookup"><span data-stu-id="0c2ad-113">To learn about how multilingual support works for learning pathways, read the [Learning pathways multilingual overview](custom_overview_ml.md)).</span></span> 

## <a name="prerequisites-to-update"></a><span data-ttu-id="0c2ad-114">更新的先决条件</span><span class="sxs-lookup"><span data-stu-id="0c2ad-114">Prerequisites to update</span></span>
<span data-ttu-id="0c2ad-115">在更新学习路径之前，必须满足以下先决条件：</span><span class="sxs-lookup"><span data-stu-id="0c2ad-115">Before updating learning pathways, the following prerequisite must be met:</span></span>
- <span data-ttu-id="0c2ad-116">更新学习路径的人必须是租户应用程序目录的网站集所有者。</span><span class="sxs-lookup"><span data-stu-id="0c2ad-116">The person updating learning pathways must be a site collection owner of the tenant App Catalog.</span></span> <span data-ttu-id="0c2ad-117">如果预配学习路径的人不是应用程序目录的网站集所有者，请 [完成这些](addappadmin.md) 说明并继续操作。</span><span class="sxs-lookup"><span data-stu-id="0c2ad-117">If the person provisioning learning pathways isn't a site collection owner of the App Catalog, [complete these instructions](addappadmin.md) and continue.</span></span> 

## <a name="set-language-settings"></a><span data-ttu-id="0c2ad-118">设置语言设置</span><span class="sxs-lookup"><span data-stu-id="0c2ad-118">Set language settings</span></span> 
<span data-ttu-id="0c2ad-119">在更新学习路径之前，请设置网站语言设置。</span><span class="sxs-lookup"><span data-stu-id="0c2ad-119">Before updating learning pathways, set the site language settings.</span></span> <span data-ttu-id="0c2ad-120">若要启用对学习路径网站的多语言支持，可以将"允许将页面和新闻翻译为多种语言"设置为 **"** 打开"，然后添加要支持该网站的语言。</span><span class="sxs-lookup"><span data-stu-id="0c2ad-120">To enable multilingual support for the learning pathways site, you can set the **Enable pages and news to be translated into multiple languages** to **On**, and then add the languages you want to support for the site.</span></span>
1.  <span data-ttu-id="0c2ad-121">从"学习路径"网站中，**从右** 上方选择"设置"，然后选择"网站 **信息"。**</span><span class="sxs-lookup"><span data-stu-id="0c2ad-121">From the Learning Pathways site, select **Settings** from the top right, and then select **Site information**.</span></span>
2.  <span data-ttu-id="0c2ad-122">在网站信息窗格底部，选择"**查看所有网站设置"。**</span><span class="sxs-lookup"><span data-stu-id="0c2ad-122">At the bottom of the site information pane, select **View all site settings**.</span></span>
3.  <span data-ttu-id="0c2ad-123">在 **"网站管理"下**，选择"**语言设置"。**</span><span class="sxs-lookup"><span data-stu-id="0c2ad-123">Under **Site Administration**, select **Language settings**.</span></span>
4.  <span data-ttu-id="0c2ad-124">在 **"启用要翻译为多种语言的页面** 和新闻"下，设置切换开关。</span><span class="sxs-lookup"><span data-stu-id="0c2ad-124">Under **Enable pages and news to be translated into multiple languages**, set the toggle switch.</span></span> 
- <span data-ttu-id="0c2ad-125">对于多语言网站，将开关滑动到 **"打开**"，然后继续"添加语言"部分。</span><span class="sxs-lookup"><span data-stu-id="0c2ad-125">For a multiligual site, slide the toggle to **On**, and then proceed to the Add Languages section.</span></span> 
- <span data-ttu-id="0c2ad-126">对于仅英文网站，将切换开关滑动到 **"关"。**</span><span class="sxs-lookup"><span data-stu-id="0c2ad-126">For an English-only site, slide the toggle to **Off**.</span></span>

### <a name="add-languages"></a><span data-ttu-id="0c2ad-127">添加语言</span><span class="sxs-lookup"><span data-stu-id="0c2ad-127">Add languages</span></span>
<span data-ttu-id="0c2ad-128">学习路径支持九种语言，应仅添加所需的语言。</span><span class="sxs-lookup"><span data-stu-id="0c2ad-128">Learning pathways supports nine languages, you should add only the languages you need.</span></span> <span data-ttu-id="0c2ad-129">在本文档中使用的示例中，将添加意大利语。</span><span class="sxs-lookup"><span data-stu-id="0c2ad-129">In the examples used in this documentation, Italian will be added.</span></span> 
- <span data-ttu-id="0c2ad-130">在 **"添加或删除网站语言"下**，开始在"选择或键入语言"中键入语言名称，或者从下拉列表中选择语言。</span><span class="sxs-lookup"><span data-stu-id="0c2ad-130">Under **Add or remove site languages**, start typing a language name in **Select or type a language**, or choose a language from the dropdown.</span></span> <span data-ttu-id="0c2ad-131">可以重复此步骤以添加多种语言。</span><span class="sxs-lookup"><span data-stu-id="0c2ad-131">You can repeat this step to add multiple languages.</span></span> <span data-ttu-id="0c2ad-132">通过返回到此页面，您随时都可以在网站中添加或删除语言。</span><span class="sxs-lookup"><span data-stu-id="0c2ad-132">You can add or remove languages from your site at any time by going back to this page.</span></span>
 
### <a name="assign-translators"></a><span data-ttu-id="0c2ad-133">分配翻译人员</span><span class="sxs-lookup"><span data-stu-id="0c2ad-133">Assign translators</span></span>
<span data-ttu-id="0c2ad-134">定义学习路径的语言设置时，可以分配翻译人员。</span><span class="sxs-lookup"><span data-stu-id="0c2ad-134">When defining Language settings for learning pathways, you can assign translators.</span></span> <span data-ttu-id="0c2ad-135">翻译人员应设置外语配置文件。</span><span class="sxs-lookup"><span data-stu-id="0c2ad-135">Translators should have a foreign language profile set up.</span></span> <span data-ttu-id="0c2ad-136">有关外语配置文件的信息，请参阅创建 [多语言通信网站、页面和新闻](https://support.office.com/article/2bb7d610-5453-41c6-a0e8-6f40b3ed750c)。</span><span class="sxs-lookup"><span data-stu-id="0c2ad-136">For more information about foreign language profiles, see [Create multilingual communication sites, pages, and news](https://support.office.com/article/2bb7d610-5453-41c6-a0e8-6f40b3ed750c).</span></span>  
- <span data-ttu-id="0c2ad-137">对于受支持的语言，请单击 **"选择或键入转换器** "，然后选择一个转换器。</span><span class="sxs-lookup"><span data-stu-id="0c2ad-137">For a supported language, click **Select or type a translator** and then select a translator.</span></span> 

## <a name="update-the-learning-pathways-web-part-package"></a><span data-ttu-id="0c2ad-138">更新学习路径 Web 部件包</span><span class="sxs-lookup"><span data-stu-id="0c2ad-138">Update the learning pathways web part package</span></span>
<span data-ttu-id="0c2ad-139">在此步骤中，您将学习路径 4.0 Web 部件上载到 SharePoint 应用程序目录，然后导航到学习路径管理页以开始更新过程。</span><span class="sxs-lookup"><span data-stu-id="0c2ad-139">In this step, you upload the learning pathways 4.0 web part to the SharePoint App Catalog, and then navigate to the learning pathways Administration page to start the update process.</span></span>

### <a name="upload-the-web-part-package"></a><span data-ttu-id="0c2ad-140">上传 Web 部件包</span><span class="sxs-lookup"><span data-stu-id="0c2ad-140">Upload the web part package</span></span>
1.  <span data-ttu-id="0c2ad-141">转到 [GitHub 自定义学习存储库](https://github.com/pnp/custom-learning-office-365/tree/master/webpart)，选择 **customlearning.sppkg，** 然后将它下载到电脑上的本地驱动器。</span><span class="sxs-lookup"><span data-stu-id="0c2ad-141">Go to the [GitHub custom learning repository](https://github.com/pnp/custom-learning-office-365/tree/master/webpart), select **customlearning.sppkg** and then download it to a local drive on your PC.</span></span> 
2.  <span data-ttu-id="0c2ad-142">如果你尚未登录，请使用租户管理员或网站集管理员帐户登录租户。</span><span class="sxs-lookup"><span data-stu-id="0c2ad-142">If you’re not already signed in, sign into your tenant with a Tenant Admin or Site Collection Admin account.</span></span> 
3.  <span data-ttu-id="0c2ad-143">单击 **"管理员**  >  **显示**  >  **所有 SharePoint**  >  **更多功能"。**</span><span class="sxs-lookup"><span data-stu-id="0c2ad-143">Click **Admin** > **Show All** > **SharePoint** > **More Features**.</span></span> 
4.  <span data-ttu-id="0c2ad-144">在"**应用"** 下，单击"**打开"。**</span><span class="sxs-lookup"><span data-stu-id="0c2ad-144">Under **Apps**, click **Open**.</span></span> 
5.  <span data-ttu-id="0c2ad-145">单击 **"应用程序目录**  >  **分发 SharePoint 应用程序"。**</span><span class="sxs-lookup"><span data-stu-id="0c2ad-145">Click **App Catalog** > **Distribute Apps for SharePoint**.</span></span> 
6.  <span data-ttu-id="0c2ad-146">单击 **上传**  >  **选择文件**。</span><span class="sxs-lookup"><span data-stu-id="0c2ad-146">Click **Upload** > **Choose Files**.</span></span> 
7.  <span data-ttu-id="0c2ad-147">选择已 **下载的 customlearning.sppkg** 文件，**单击"确定**""部署  >  **"。**</span><span class="sxs-lookup"><span data-stu-id="0c2ad-147">Select the **customlearning.sppkg** file you downloaded, click **OK** > **Deploy**.</span></span> 

### <a name="complete-the-update"></a><span data-ttu-id="0c2ad-148">完成更新</span><span class="sxs-lookup"><span data-stu-id="0c2ad-148">Complete the update</span></span>
1.  <span data-ttu-id="0c2ad-149">从"学习路径"网站，从"开始" **菜单中选择** "学习路径 **管理** "。</span><span class="sxs-lookup"><span data-stu-id="0c2ad-149">From the Learning Pathways site, select **Learning pathways administration** from the **Home** menu.</span></span> 
2.  <span data-ttu-id="0c2ad-150">你将看到一条提示，询问是否要更新。</span><span class="sxs-lookup"><span data-stu-id="0c2ad-150">You’ll see a prompt asking if you want to update.</span></span> 
<span data-ttu-id="0c2ad-151">![custom_update_adminprompt_ml.png](media/custom_update_adminprompt_ml.png)</span><span class="sxs-lookup"><span data-stu-id="0c2ad-151">![custom_update_adminprompt_ml.png](media/custom_update_adminprompt_ml.png)</span></span>
3.  <span data-ttu-id="0c2ad-152">单击“**开始**”。</span><span class="sxs-lookup"><span data-stu-id="0c2ad-152">Click **Start**.</span></span> 
4. <span data-ttu-id="0c2ad-153">更新完成后，单击 **关闭。**</span><span class="sxs-lookup"><span data-stu-id="0c2ad-153">When the update is complete, click **Close**.</span></span> 

### <a name="next-steps"></a><span data-ttu-id="0c2ad-154">后续步骤</span><span class="sxs-lookup"><span data-stu-id="0c2ad-154">Next Steps</span></span>
- <span data-ttu-id="0c2ad-155">浏览 [网站和](custom_exploresite.md) Web 部件中提供的默认内容。</span><span class="sxs-lookup"><span data-stu-id="0c2ad-155">Explore the [default content](custom_exploresite.md) provided in the site and web part.</span></span>
- <span data-ttu-id="0c2ad-156">有关翻译网站页面的信息，请参阅翻译 [网站页面](custom_translate_page_ml.md)。</span><span class="sxs-lookup"><span data-stu-id="0c2ad-156">For more information about translating site pages, see [Translate site pages](custom_translate_page_ml.md).</span></span> 

