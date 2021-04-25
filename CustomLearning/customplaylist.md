---
author: karuanag
ms.author: karuanag
manager: alexb
title: 自定义和共享播放列表
ms.date: 02/10/2019
description: 从现有内容或新 SharePoint 页面创建自定义播放列表
ms.service: sharepoint-online
audience: itpro
ms.topic: article
ms.openlocfilehash: 31a0e5524181d26f4d62ae7206636c9e553b6f8f
ms.sourcegitcommit: 97e175e5ff5b6a9e0274d5ec9b39fdf7e18eb387
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/25/2021
ms.locfileid: "52000208"
---
# <a name="customize-and-share-playlists"></a><span data-ttu-id="33b4d-103">自定义和共享播放列表</span><span class="sxs-lookup"><span data-stu-id="33b4d-103">Customize and share playlists</span></span>

## <a name="create-a-playlist"></a><span data-ttu-id="33b4d-104">创建播放列表</span><span class="sxs-lookup"><span data-stu-id="33b4d-104">Create a Playlist</span></span>

<span data-ttu-id="33b4d-105">播放列表是"资产"的一个复杂过程。</span><span class="sxs-lookup"><span data-stu-id="33b4d-105">A playlist is a compliation of "assets".</span></span> <span data-ttu-id="33b4d-106">"资产"是 SharePoint 页面或 Microsoft 培训内容的现有项。</span><span class="sxs-lookup"><span data-stu-id="33b4d-106">An "asset" is a SharePoint page or existing item of Microsoft training content.</span></span> <span data-ttu-id="33b4d-107">创建播放列表时，选择一起为用户创建学习路径的资产。</span><span class="sxs-lookup"><span data-stu-id="33b4d-107">When you create a playlist you select assets that go together to create a learning path for your user.</span></span>  

<span data-ttu-id="33b4d-108">添加 SharePoint 页面的好处是，您可以使用组织中托管的 YouTube 视频创建 SharePoint 页面。</span><span class="sxs-lookup"><span data-stu-id="33b4d-108">The benefit of adding SharePoint pages is that you can create SharePoint pages with a YouTube videos or videos hosted in your organization.</span></span> <span data-ttu-id="33b4d-109">您还可以使用 Forms 或其他 Office 365 内容创建页面。</span><span class="sxs-lookup"><span data-stu-id="33b4d-109">You can also create pages with Forms or other Office 365 content.</span></span>  

#### <a name="step-1-create-a-sharepoint-page-for-your-playlist"></a><span data-ttu-id="33b4d-110">步骤 1：为播放列表创建 SharePoint 页面</span><span class="sxs-lookup"><span data-stu-id="33b4d-110">Step 1: Create a SharePoint page for your playlist</span></span>
<span data-ttu-id="33b4d-111">此示例首先创建一个要添加到播放列表的 SharePoint 页面。</span><span class="sxs-lookup"><span data-stu-id="33b4d-111">In this example, we’ll first create a SharePoint page to add to the playlist.</span></span> <span data-ttu-id="33b4d-112">我们将创建一个包含 YouTube 视频 Web 部件和文本 Web 部件的页面。</span><span class="sxs-lookup"><span data-stu-id="33b4d-112">We’ll create a page with a YouTube video web part and Text web part.</span></span>  <span data-ttu-id="33b4d-113">这些说明假定你使用的是 SharePoint Online 服务。</span><span class="sxs-lookup"><span data-stu-id="33b4d-113">These instructions assume you are using the SharePoint Online service.</span></span> 

#### <a name="create-a-new-page"></a><span data-ttu-id="33b4d-114">创建新页面</span><span class="sxs-lookup"><span data-stu-id="33b4d-114">Create a new page</span></span>
1.  <span data-ttu-id="33b4d-115">Select the Settings menu > Site Contents > Site Pages > New > Site Page.</span><span class="sxs-lookup"><span data-stu-id="33b4d-115">Select the Settings menu > Site Contents > Site Pages > New > Site Page.</span></span>
2.  <span data-ttu-id="33b4d-116">在标题区域中，键入使用 Teams 命令框</span><span class="sxs-lookup"><span data-stu-id="33b4d-116">In the title area, type Use the Teams command box</span></span>
3.  <span data-ttu-id="33b4d-117">选择"添加新节"，然后选择"两列"。</span><span class="sxs-lookup"><span data-stu-id="33b4d-117">Select the Add a new section, and then select Two Columns.</span></span>

![两列添加](media/clo365addtwocolumn.png)

4.  <span data-ttu-id="33b4d-119">在左侧框中，选择"添加新 Web 部件"，然后选择"嵌入"。</span><span class="sxs-lookup"><span data-stu-id="33b4d-119">In the left-hand box, select Add a new web part, and then select Embed.</span></span> 
5.  <span data-ttu-id="33b4d-120">在 Web 浏览器中，转到此 URL https://youtu.be/wYrRCRphrp0 并获取视频的嵌入代码。</span><span class="sxs-lookup"><span data-stu-id="33b4d-120">In a Web browser, go to this URL https://youtu.be/wYrRCRphrp0 and get the embed code for the video.</span></span> 
6.  <span data-ttu-id="33b4d-121">在 SharePoint Web 部件中，选择"添加嵌入代码"，然后将其粘贴到"嵌入"框中。</span><span class="sxs-lookup"><span data-stu-id="33b4d-121">In the SharePoint Web part, select Add Embed code and then paste it into the Embed box.</span></span> 
7.  <span data-ttu-id="33b4d-122">在右侧框中，选择"添加新 Web 部件"，然后选择"文本"。</span><span class="sxs-lookup"><span data-stu-id="33b4d-122">In the right-hand box, select Add a new web part, and then select Text.</span></span> 
8.  <span data-ttu-id="33b4d-123">在 Web 浏览器中，转到此 URL： https://support.office.com/article/13c4e429-7324-4886-b377-5dbed539193b 并复制试用！</span><span class="sxs-lookup"><span data-stu-id="33b4d-123">In a Web browser, go to this URL: https://support.office.com/article/13c4e429-7324-4886-b377-5dbed539193b and copy the Try it!</span></span> <span data-ttu-id="33b4d-124">页面中的说明，并将其粘贴到文本 Web 部件中。</span><span class="sxs-lookup"><span data-stu-id="33b4d-124">Instructions from the page and paste them into the Text Web part.</span></span> <span data-ttu-id="33b4d-125">页面应如下所示。</span><span class="sxs-lookup"><span data-stu-id="33b4d-125">Your page should look like the following.</span></span> 
<span data-ttu-id="33b4d-126">![嵌入页面](media/clo365teamscommandbox.png)</span><span class="sxs-lookup"><span data-stu-id="33b4d-126">![Embed page](media/clo365teamscommandbox.png)</span></span>
9.  <span data-ttu-id="33b4d-127">单击 **"** 发布"，然后复制页面的 URL 并将其粘贴到记事本中</span><span class="sxs-lookup"><span data-stu-id="33b4d-127">Click **Publish**, and then copy the URL of the page and paste it in Notepad</span></span>

#### <a name="step-2-create-the-playlist"></a><span data-ttu-id="33b4d-128">步骤 2：创建播放列表</span><span class="sxs-lookup"><span data-stu-id="33b4d-128">Step 2: Create the Playlist</span></span>

1. <span data-ttu-id="33b4d-129">导航到 **网站体验中的** "自定义学习管理"页。</span><span class="sxs-lookup"><span data-stu-id="33b4d-129">Navigate to the **Custom Learning Administration** page in your site experience.</span></span>
<span data-ttu-id="33b4d-130">![选择"自定义学习管理"的屏幕。](media/custom_admin.png)</span><span class="sxs-lookup"><span data-stu-id="33b4d-130">![Screen where you select Custom Learning Administration.](media/custom_admin.png)</span></span>
1. <span data-ttu-id="33b4d-131">确保 **已选择** "类别"</span><span class="sxs-lookup"><span data-stu-id="33b4d-131">Make sure **Category** is selected</span></span> 
1. <span data-ttu-id="33b4d-132">单击要显示新播放列表的类别</span><span class="sxs-lookup"><span data-stu-id="33b4d-132">Click on the category where you'd like your new playlist to appear</span></span>
1. <span data-ttu-id="33b4d-133">在类别名称旁边，单击加号"窗口"，并突出显示 ![ "类别"选项和"加号"。](media/custom_addplay.png)</span><span class="sxs-lookup"><span data-stu-id="33b4d-133">Next to the category name, click on the plus symbol ![Window with the Category option and the Plus sign highlighted.](media/custom_addplay.png)</span></span>

1. <span data-ttu-id="33b4d-134">填写值，如下面的示例所示， **然后选择创建**。</span><span class="sxs-lookup"><span data-stu-id="33b4d-134">Fill in the values as shown in the example below and select **Create**.</span></span> 
<span data-ttu-id="33b4d-135">![输入播放列表详细信息的页面。](media/custom_details.png)</span><span class="sxs-lookup"><span data-stu-id="33b4d-135">![Page where you enter playlist details.](media/custom_details.png)</span></span>
- <span data-ttu-id="33b4d-136">**Title** - 播放列表的显示名称</span><span class="sxs-lookup"><span data-stu-id="33b4d-136">**Title** - Display name of the playlist</span></span>
- <span data-ttu-id="33b4d-137">**说明** - 将学习哪些内容的信息</span><span class="sxs-lookup"><span data-stu-id="33b4d-137">**Description** - Information about what will be learned</span></span>
- <span data-ttu-id="33b4d-138">**类别** - 根据初始选择预选</span><span class="sxs-lookup"><span data-stu-id="33b4d-138">**Category** - Preselected based on your initial selection</span></span>
- <span data-ttu-id="33b4d-139">**子类别** - 根据你的选择预选</span><span class="sxs-lookup"><span data-stu-id="33b4d-139">**Sub Category** - Preselected based on your intial selection</span></span>
- <span data-ttu-id="33b4d-140">**技术** - 选择（如果适用）</span><span class="sxs-lookup"><span data-stu-id="33b4d-140">**Technology** - Select as applicable</span></span>
- <span data-ttu-id="33b4d-141">**Level** - 初学者、Intermidate 或 Advanced</span><span class="sxs-lookup"><span data-stu-id="33b4d-141">**Level** - Beginner, Intermidate or Advanced</span></span>
- <span data-ttu-id="33b4d-142">**访问** 群体 - 这允许您基于 Microsoft 提供的角色的预定义列表来定位内容。</span><span class="sxs-lookup"><span data-stu-id="33b4d-142">**Audience** - This allows you to target content based on a pre-defined list of roles provided by Microsoft.</span></span>

6. <span data-ttu-id="33b4d-143">单击 **"保存详细信息"**</span><span class="sxs-lookup"><span data-stu-id="33b4d-143">Click **Save Detail**</span></span>

> [!TIP]
> <span data-ttu-id="33b4d-144">你可以自定义播放列表的图标图像。</span><span class="sxs-lookup"><span data-stu-id="33b4d-144">You can customize the icon image for your playlist.</span></span>  <span data-ttu-id="33b4d-145">单击图像图标并插入以前上载的图像的 URL。</span><span class="sxs-lookup"><span data-stu-id="33b4d-145">Click the image icon and insert an URL of a previously uploaded image.</span></span>  <span data-ttu-id="33b4d-146">确保图像位于自定义学习网站集内或所有用户都将有权访问该文件的另一个位置。</span><span class="sxs-lookup"><span data-stu-id="33b4d-146">Make sure the image is located within the Custom Learning site collection or in another location that all users will have access to the file.</span></span>  
<span data-ttu-id="33b4d-147">![选择图像窗口。](media/custom_image.png)</span><span class="sxs-lookup"><span data-stu-id="33b4d-147">![Choose an image window.](media/custom_image.png)</span></span>

#### <a name="step-3-add-assets-to-the-playlist"></a><span data-ttu-id="33b4d-148">步骤 3：将资产添加到播放列表</span><span class="sxs-lookup"><span data-stu-id="33b4d-148">Step 3: Add assets to the playlist</span></span>
<span data-ttu-id="33b4d-149">在此步骤中，你将从 Microsoft 和你创建的 SharePoint 页面将现有资源添加到播放列表。</span><span class="sxs-lookup"><span data-stu-id="33b4d-149">In this step, you’ll add existing assets from Microsoft and the SharePoint page you created to the playlist.</span></span> 

1. <span data-ttu-id="33b4d-150">保存播放列表的详细信息后，可以使用"搜索现有资源"。</span><span class="sxs-lookup"><span data-stu-id="33b4d-150">Once you have saved the details for your Playlist you can use the Search for Existing Assets.</span></span>
1. <span data-ttu-id="33b4d-151">**输入任何搜索词** 以查看可从其他播放列表访问的预定义资产列表。</span><span class="sxs-lookup"><span data-stu-id="33b4d-151">**Enter in any search term** to see a list of predefined assets that are available from other playlists.</span></span> <span data-ttu-id="33b4d-152">**单击资产名称** 以将资产添加到新播放列表中。</span><span class="sxs-lookup"><span data-stu-id="33b4d-152">**Click on the name** of an asset to include it in your new playlist.</span></span><br/>
<span data-ttu-id="33b4d-153">![播放列表资产页面](media/custom_slist.png)</span><span class="sxs-lookup"><span data-stu-id="33b4d-153">![Playlist assets page](media/custom_slist.png)</span></span>

<span data-ttu-id="33b4d-154">还可以添加之前创建的 SharePoint 页面，或从头开始创建一个体验页面。</span><span class="sxs-lookup"><span data-stu-id="33b4d-154">You can also add the SharePoint page you created earlier or create one from scratch in the experience.</span></span>

1. <span data-ttu-id="33b4d-155">单击" **播放列表资产"** 对话框中的"新建资产"选项。</span><span class="sxs-lookup"><span data-stu-id="33b4d-155">Click on the **New Asset** option in the Playlist Assets dialog.</span></span>
1. <span data-ttu-id="33b4d-156">为资产提供 **标题**。</span><span class="sxs-lookup"><span data-stu-id="33b4d-156">Give your asset a **Title**.</span></span> <span data-ttu-id="33b4d-157">输入后，将显示其他选项。</span><span class="sxs-lookup"><span data-stu-id="33b4d-157">Once entered, additional options will display.</span></span>
<span data-ttu-id="33b4d-158">![输入标题和其他详细信息的表单。](media/custom_newpage.png)</span><span class="sxs-lookup"><span data-stu-id="33b4d-158">![Form where you enter your title and additional details.](media/custom_newpage.png)</span></span>
1. <span data-ttu-id="33b4d-159">现在可以在 SharePoint Online 中创建新的资产页面，或输入现有页面的 URL 以将其添加到自定义播放列表。</span><span class="sxs-lookup"><span data-stu-id="33b4d-159">You can now create a new asset page in SharePoint Online or enter in the URL of an existing page to add it to your custom playlist.</span></span> 
1. <span data-ttu-id="33b4d-160">**"\*\*\*\*类别"、"** 子类别"和"技术"字段将基于你之前对此播放列表的选择进行预填充。 </span><span class="sxs-lookup"><span data-stu-id="33b4d-160">**Category**, **Sub Category** and **Technology** fields will be pre-populated based on your previous selections for this playlist.</span></span>
1. <span data-ttu-id="33b4d-161">为此单个资产的"级别"和"访问群体"进行适当的选择。</span><span class="sxs-lookup"><span data-stu-id="33b4d-161">Make the appropriate selections for Level and Audience for this individual asset.</span></span>  
1. <span data-ttu-id="33b4d-162">单击 **"保存资产** "将其添加到自定义播放列表</span><span class="sxs-lookup"><span data-stu-id="33b4d-162">Click **Save Asset** to add it to the custom playlist</span></span>
1. <span data-ttu-id="33b4d-163">重复这些步骤（搜索或添加单个页面）直到播放列表完成。</span><span class="sxs-lookup"><span data-stu-id="33b4d-163">Repeat these steps, either searching or adding individual pages, until your playlist is complete.</span></span> 
1. <span data-ttu-id="33b4d-164">单击 **关闭播放列表** 以保存</span><span class="sxs-lookup"><span data-stu-id="33b4d-164">Click **Close Playlist** to save</span></span>

<span data-ttu-id="33b4d-165">你具有此内容的播放列表现在将在你已安装/嵌入自定义学习 Web 部件的任何位置可用。</span><span class="sxs-lookup"><span data-stu-id="33b4d-165">Your playlist with this content will now be available anywhere you have installed / embedded the Custom Learning webpart.</span></span> 

> [!NOTE]
> <span data-ttu-id="33b4d-166">如果在关闭播放列表后出错，可以通过单击播放列表名称旁边的 X 将其从类别中删除。</span><span class="sxs-lookup"><span data-stu-id="33b4d-166">If you make a mistake once you have closed the playlist, you can delete it from the category by clicking the X next to the playlist name.</span></span>  

#### <a name="things-to-think-about"></a><span data-ttu-id="33b4d-167">要思考的事情</span><span class="sxs-lookup"><span data-stu-id="33b4d-167">Things to Think About</span></span>

<span data-ttu-id="33b4d-168">自定义播放列表可用于帮助最终用户完成各种任务。</span><span class="sxs-lookup"><span data-stu-id="33b4d-168">Custom playlists can be used to assist your end users in a variety of tasks.</span></span>  <span data-ttu-id="33b4d-169">您是否有请假请求表单？</span><span class="sxs-lookup"><span data-stu-id="33b4d-169">Do you have a time off request form?</span></span>  <span data-ttu-id="33b4d-170">请求硬件设备的表单</span><span class="sxs-lookup"><span data-stu-id="33b4d-170">A form to request hardware equipment?</span></span>  <span data-ttu-id="33b4d-171">可以将任何现有培训资产编入体验。</span><span class="sxs-lookup"><span data-stu-id="33b4d-171">Any existing training assets can be programmed into the experience.</span></span>  

## <a name="share-playlists"></a><span data-ttu-id="33b4d-172">共享播放列表</span><span class="sxs-lookup"><span data-stu-id="33b4d-172">Share Playlists</span></span>

1. <span data-ttu-id="33b4d-173">导航到 Web 部件或网站体验内的任何播放列表</span><span class="sxs-lookup"><span data-stu-id="33b4d-173">Navigate to any playlist within the webpart or site experience</span></span>
1. <span data-ttu-id="33b4d-174">在左上角，你将看到三个图标</span><span class="sxs-lookup"><span data-stu-id="33b4d-174">In the upper left hand corner you will see three icons</span></span>
1. <span data-ttu-id="33b4d-175">单击表示链接的图标</span><span class="sxs-lookup"><span data-stu-id="33b4d-175">Click on the icon representing a link</span></span>
1. <span data-ttu-id="33b4d-176">将 URL 复制到播放列表 ![ 屏幕，单击 URL 旁边的"复制"。](media/share.png)</span><span class="sxs-lookup"><span data-stu-id="33b4d-176">Copy the URL to the playlist ![Screen where you click Copy next to the URL.](media/share.png)</span></span>
<span data-ttu-id="33b4d-177">现在可以在网站导航中插入此 URL，或在其他通信中利用此 URL 将员工直接添加到该播放列表中。</span><span class="sxs-lookup"><span data-stu-id="33b4d-177">This URL can now be inserted in your site navigation or utilized in other communications to take your employees directly to that playlist.</span></span> 

### <a name="next-steps---drive-adoption"></a><span data-ttu-id="33b4d-178">下一步 - [推动采用](driveadoption.md)</span><span class="sxs-lookup"><span data-stu-id="33b4d-178">Next Steps - [Drive Adoption](driveadoption.md)</span></span>
