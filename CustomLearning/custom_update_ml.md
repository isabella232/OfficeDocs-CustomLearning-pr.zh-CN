---
author: pkrebs
ms.author: pkrebs
title: 更新多语言支持的学习路径
ms.date: 05/20/2019
description: 更新多语言支持的学习路径
ROBOTS: NOINDEX, NOFOLLOW
ms.openlocfilehash: 37a9b77ee45b8ae1ae4973f171c32de11fb530e1
ms.sourcegitcommit: 1f080ed4cf3687f922907304db3fd7a06aa9d501
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2020
ms.locfileid: "45031698"
---
# <a name="update-learning-pathways-for-multilingual-support"></a><span data-ttu-id="370b6-103">更新多语言支持的学习路径</span><span class="sxs-lookup"><span data-stu-id="370b6-103">Update learning pathways for multilingual support</span></span>
<span data-ttu-id="370b6-104">如果您有现有的学习路径网站，则可以更新它以实现多语言支持。</span><span class="sxs-lookup"><span data-stu-id="370b6-104">If you have an existing Learning Pathways site, you can update it for multilingual support.</span></span> <span data-ttu-id="370b6-105">若要更新到多语言4.0 版本的学习路径，请将 web 部件包 customlearning （.sppkg）上传到 SharePoint 租户应用程序目录。</span><span class="sxs-lookup"><span data-stu-id="370b6-105">To update learning pathways to the multilingual 4.0 version, you upload the web part package, customlearning.sppkg, to the SharePoint tenant App Catalog.</span></span> <span data-ttu-id="370b6-106">更新学习路径时：</span><span class="sxs-lookup"><span data-stu-id="370b6-106">When you update learning pathways:</span></span>  

- <span data-ttu-id="370b6-107">任何以前创建的自定义播放列表和资产都将保留</span><span class="sxs-lookup"><span data-stu-id="370b6-107">Any previously created custom playlists and assets are maintained</span></span>
- <span data-ttu-id="370b6-108">保留隐藏或显示内容的设置</span><span class="sxs-lookup"><span data-stu-id="370b6-108">Settings to hide or show content are maintained</span></span>
- <span data-ttu-id="370b6-109">"学习路径" SharePoint 模板保持不变</span><span class="sxs-lookup"><span data-stu-id="370b6-109">The learning pathways SharePoint template is left unchanged</span></span>
- <span data-ttu-id="370b6-110">不翻译学习路径网站页面。</span><span class="sxs-lookup"><span data-stu-id="370b6-110">The learning pathways site pages aren't translated.</span></span> <span data-ttu-id="370b6-111">此工作必须手动完成</span><span class="sxs-lookup"><span data-stu-id="370b6-111">This work must be done manually</span></span>

## <a name="read-the-learning-pathways-multilingual-overview"></a><span data-ttu-id="370b6-112">阅读学习路径多语言概述</span><span class="sxs-lookup"><span data-stu-id="370b6-112">Read the learning pathways multilingual overview</span></span>
<span data-ttu-id="370b6-113">若要了解多语言支持对学习路径的工作方式，请阅读[学习路径多语言概述](custom_overview_ml.md)）。</span><span class="sxs-lookup"><span data-stu-id="370b6-113">To learn about how multilingual support works for learning pathways, read the [Learning pathways multilingual overview](custom_overview_ml.md)).</span></span> 

## <a name="prerequisites-to-update"></a><span data-ttu-id="370b6-114">要更新的先决条件</span><span class="sxs-lookup"><span data-stu-id="370b6-114">Prerequisites to update</span></span>
<span data-ttu-id="370b6-115">在更新学习路径之前，必须满足以下先决条件：</span><span class="sxs-lookup"><span data-stu-id="370b6-115">Before updating learning pathways, the following prerequisite must be met:</span></span>
- <span data-ttu-id="370b6-116">更新学习路径的人员必须是租户应用程序目录的网站集所有者。</span><span class="sxs-lookup"><span data-stu-id="370b6-116">The person updating learning pathways must be a site collection owner of the tenant App Catalog.</span></span> <span data-ttu-id="370b6-117">如果人员设置学习路径不是应用程序目录的网站集所有者，请[完成这些说明](addappadmin.md)并继续。</span><span class="sxs-lookup"><span data-stu-id="370b6-117">If the person provisioning learning pathways isn't a site collection owner of the App Catalog, [complete these instructions](addappadmin.md) and continue.</span></span> 

## <a name="set-language-settings"></a><span data-ttu-id="370b6-118">设置语言设置</span><span class="sxs-lookup"><span data-stu-id="370b6-118">Set language settings</span></span> 
<span data-ttu-id="370b6-119">在更新学习路径之前，请设置 "网站语言设置"。</span><span class="sxs-lookup"><span data-stu-id="370b6-119">Before updating learning pathways, set the site language settings.</span></span> <span data-ttu-id="370b6-120">若要对学习路径网站启用多语言支持，您可以将 "**启用页面和新闻**" 设置为 "转换为多种语言 **"，然后**添加要为网站支持的语言。</span><span class="sxs-lookup"><span data-stu-id="370b6-120">To enable multilingual support for the learning pathways site, you can set the **Enable pages and news to be translated into multiple languages** to **On**, and then add the languages you want to support for the site.</span></span>
1.  <span data-ttu-id="370b6-121">从 "学习路径" 网站中，从右上部选择 "**设置**"，然后选择 "**网站信息**"。</span><span class="sxs-lookup"><span data-stu-id="370b6-121">From the Learning Pathways site, select **Settings** from the top right, and then select **Site information**.</span></span>
2.  <span data-ttu-id="370b6-122">在 "网站信息" 窗格的底部，选择 "**查看所有网站设置**"。</span><span class="sxs-lookup"><span data-stu-id="370b6-122">At the bottom of the site information pane, select **View all site settings**.</span></span>
3.  <span data-ttu-id="370b6-123">在 "**网站管理**" 下，选择 "**语言设置**"。</span><span class="sxs-lookup"><span data-stu-id="370b6-123">Under **Site Administration**, select **Language settings**.</span></span>
4.  <span data-ttu-id="370b6-124">在 "**允许将页面和新闻转换为多种语言**" 下，设置切换开关。</span><span class="sxs-lookup"><span data-stu-id="370b6-124">Under **Enable pages and news to be translated into multiple languages**, set the toggle switch.</span></span> 
- <span data-ttu-id="370b6-125">对于 multiligual 网站，将切换滑到 **"开**"，然后继续转到 "添加语言" 部分。</span><span class="sxs-lookup"><span data-stu-id="370b6-125">For a multiligual site, slide the toggle to **On**, and then proceed to the Add Languages section.</span></span> 
- <span data-ttu-id="370b6-126">对于仅英语的网站，将开关滑到 "**关闭**"。</span><span class="sxs-lookup"><span data-stu-id="370b6-126">For an English-only site, slide the toggle to **Off**.</span></span>

### <a name="add-languages"></a><span data-ttu-id="370b6-127">添加语言</span><span class="sxs-lookup"><span data-stu-id="370b6-127">Add languages</span></span>
<span data-ttu-id="370b6-128">学习路径支持九种语言，您应该只添加所需的语言。</span><span class="sxs-lookup"><span data-stu-id="370b6-128">Learning pathways supports nine languages, you should add only the languages you need.</span></span> <span data-ttu-id="370b6-129">在本文档中使用的示例中，将添加意大利语。</span><span class="sxs-lookup"><span data-stu-id="370b6-129">In the examples used in this documentation, Italian will be added.</span></span> 
- <span data-ttu-id="370b6-130">在 "**添加或删除网站语言**" 下，开始在 "**选择" 或 "键入语言**" 中键入语言名称，或从下拉列表中选择一种语言。</span><span class="sxs-lookup"><span data-stu-id="370b6-130">Under **Add or remove site languages**, start typing a language name in **Select or type a language**, or choose a language from the dropdown.</span></span> <span data-ttu-id="370b6-131">您可以重复此步骤以添加多种语言。</span><span class="sxs-lookup"><span data-stu-id="370b6-131">You can repeat this step to add multiple languages.</span></span> <span data-ttu-id="370b6-132">您可以通过返回到此页随时在网站中添加或删除语言。</span><span class="sxs-lookup"><span data-stu-id="370b6-132">You can add or remove languages from your site at any time by going back to this page.</span></span>
 
### <a name="assign-translators"></a><span data-ttu-id="370b6-133">分配翻译人员</span><span class="sxs-lookup"><span data-stu-id="370b6-133">Assign translators</span></span>
<span data-ttu-id="370b6-134">在为学习路径定义语言设置时，您可以分配翻译者。</span><span class="sxs-lookup"><span data-stu-id="370b6-134">When defining Language settings for learning pathways, you can assign translators.</span></span> <span data-ttu-id="370b6-135">翻译人员应设置外部语言配置文件。</span><span class="sxs-lookup"><span data-stu-id="370b6-135">Translators should have a foreign language profile set up.</span></span> <span data-ttu-id="370b6-136">有关外部语言配置文件的详细信息，请参阅[创建多语言通信网站、页面和新闻](https://support.office.com/article/2bb7d610-5453-41c6-a0e8-6f40b3ed750c)。</span><span class="sxs-lookup"><span data-stu-id="370b6-136">For more information about foreign language profiles, see [Create multilingual communication sites, pages, and news](https://support.office.com/article/2bb7d610-5453-41c6-a0e8-6f40b3ed750c).</span></span>  
- <span data-ttu-id="370b6-137">对于受支持的语言，请单击 "**选择或键入翻译人员**"，然后选择一个转换器。</span><span class="sxs-lookup"><span data-stu-id="370b6-137">For a supported language, click **Select or type a translator** and then select a translator.</span></span> 

## <a name="update-the-learning-pathways-web-part-package"></a><span data-ttu-id="370b6-138">更新 "学习路径" web 部件包</span><span class="sxs-lookup"><span data-stu-id="370b6-138">Update the learning pathways web part package</span></span>
<span data-ttu-id="370b6-139">在此步骤中，将 "学习路径 4.0" web 部件上传到 SharePoint 应用程序目录，然后导航到 "学习路径管理" 页以启动更新过程。</span><span class="sxs-lookup"><span data-stu-id="370b6-139">In this step, you upload the learning pathways 4.0 web part to the SharePoint App Catalog, and then navigate to the learning pathways Administration page to start the update process.</span></span>

### <a name="upload-the-web-part-package"></a><span data-ttu-id="370b6-140">上载 web 部件包</span><span class="sxs-lookup"><span data-stu-id="370b6-140">Upload the web part package</span></span>
1.  <span data-ttu-id="370b6-141">转到 "团队中的多语言共享位置"，并将**customlearning**下载到电脑上的本地驱动器。</span><span class="sxs-lookup"><span data-stu-id="370b6-141">Go to the multilingual share location in Teams and download **customlearning.sppkg** to a local drive on your PC.</span></span> 
2.  <span data-ttu-id="370b6-142">如果您尚未登录，请使用租户管理员或网站集管理员帐户登录到你的租户。</span><span class="sxs-lookup"><span data-stu-id="370b6-142">If you’re not already signed in, sign into your tenant with a Tenant Admin or Site Collection Admin account.</span></span> 
3.  <span data-ttu-id="370b6-143">单击 "**管理**  >  **显示所有**  >  **SharePoint**  >  **更多功能**"。</span><span class="sxs-lookup"><span data-stu-id="370b6-143">Click **Admin** > **Show All** > **SharePoint** > **More Features**.</span></span> 
4.  <span data-ttu-id="370b6-144">在 "**应用**" 下，单击 "**打开**"。</span><span class="sxs-lookup"><span data-stu-id="370b6-144">Under **Apps**, click **Open**.</span></span> 
5.  <span data-ttu-id="370b6-145">单击 "**应用程序目录**  >  **分发 SharePoint 相关应用**程序"。</span><span class="sxs-lookup"><span data-stu-id="370b6-145">Click **App Catalog** > **Distribute Apps for SharePoint**.</span></span> 
6.  <span data-ttu-id="370b6-146">单击 "**上载**  >  **选择文件**"。</span><span class="sxs-lookup"><span data-stu-id="370b6-146">Click **Upload** > **Choose Files**.</span></span> 
7.  <span data-ttu-id="370b6-147">选择您下载的**customlearning**文件，然后单击 **"确定**  >  **部署**"。</span><span class="sxs-lookup"><span data-stu-id="370b6-147">Select the **customlearning.sppkg** file you downloaded, click **OK** > **Deploy**.</span></span> 

### <a name="complete-the-update"></a><span data-ttu-id="370b6-148">完成更新</span><span class="sxs-lookup"><span data-stu-id="370b6-148">Complete the update</span></span>
1.  <span data-ttu-id="370b6-149">从 "学习路径" 网站中，从 "**主页**" 菜单中选择 "**学习路径管理**"。</span><span class="sxs-lookup"><span data-stu-id="370b6-149">From the Learning Pathways site, select **Learning pathways administration** from the **Home** menu.</span></span> 
2.  <span data-ttu-id="370b6-150">你将看到一条提示，询问你是否要更新。</span><span class="sxs-lookup"><span data-stu-id="370b6-150">You’ll see a prompt asking if you want to update.</span></span> 
<span data-ttu-id="370b6-151">![custom_update_adminprompt_ml.png](media/custom_update_adminprompt_ml.png)</span><span class="sxs-lookup"><span data-stu-id="370b6-151">![custom_update_adminprompt_ml.png](media/custom_update_adminprompt_ml.png)</span></span>
3.  <span data-ttu-id="370b6-152">单击“**开始**”。</span><span class="sxs-lookup"><span data-stu-id="370b6-152">Click **Start**.</span></span> 
4. <span data-ttu-id="370b6-153">更新完成后，单击 "**关闭**"。</span><span class="sxs-lookup"><span data-stu-id="370b6-153">When the update is complete, click **Close**.</span></span> 

### <a name="next-steps"></a><span data-ttu-id="370b6-154">后续步骤</span><span class="sxs-lookup"><span data-stu-id="370b6-154">Next Steps</span></span>
- <span data-ttu-id="370b6-155">浏览网站和 web 部件中提供的[默认内容](custom_exploresite.md)。</span><span class="sxs-lookup"><span data-stu-id="370b6-155">Explore the [default content](custom_exploresite.md) provided in the site and web part.</span></span>
- <span data-ttu-id="370b6-156">有关转换网站页面的详细信息，请参阅[翻译网站页面](custom_translate_page_ml.md)。</span><span class="sxs-lookup"><span data-stu-id="370b6-156">For more information about translating site pages, see [Translate site pages](custom_translate_page_ml.md).</span></span> 

