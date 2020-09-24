---
author: karuanag
ms.author: karuanag
title: 自定义和共享播放列表
ms.date: 02/10/2019
description: 从现有内容或新 SharePoint 页面创建自定义播放列表
ms.service: sharepoint online
ms.openlocfilehash: 6258668b417ba496c7ac75e36ce2bc1f1dae27a5
ms.sourcegitcommit: ee4aebf60893887ae95a1294a9ad8975539ea762
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/23/2020
ms.locfileid: "48233804"
---
# <a name="customize-and-share-playlists"></a><span data-ttu-id="3461d-103">自定义和共享播放列表</span><span class="sxs-lookup"><span data-stu-id="3461d-103">Customize and Share Playlists</span></span>

## <a name="create-a-playlist"></a><span data-ttu-id="3461d-104">创建播放列表</span><span class="sxs-lookup"><span data-stu-id="3461d-104">Create a Playlist</span></span>

<span data-ttu-id="3461d-105">播放列表是 "资产" 的 compliation。</span><span class="sxs-lookup"><span data-stu-id="3461d-105">A playlist is a compliation of "assets".</span></span> <span data-ttu-id="3461d-106">"资源" 是 SharePoint 页面或 Microsoft 培训内容的现有项目。</span><span class="sxs-lookup"><span data-stu-id="3461d-106">An "asset" is a SharePoint page or existing item of Microsoft training content.</span></span> <span data-ttu-id="3461d-107">创建播放列表时，选择的资产将一起为您的用户创建学习路径。</span><span class="sxs-lookup"><span data-stu-id="3461d-107">When you create a playlist you select assets that go together to create a learning path for your user.</span></span>  

<span data-ttu-id="3461d-108">添加 SharePoint 页面的好处在于，您可以使用组织中托管的 YouTube 视频或视频创建 SharePoint 页面。</span><span class="sxs-lookup"><span data-stu-id="3461d-108">The benefit of adding SharePoint pages is that you can create SharePoint pages with a YouTube videos or videos hosted in your organization.</span></span> <span data-ttu-id="3461d-109">您还可以使用表单或其他 Office 365 内容创建页面。</span><span class="sxs-lookup"><span data-stu-id="3461d-109">You can also create pages with Forms or other Office 365 content.</span></span>  

#### <a name="step-1-create-a-sharepoint-page-for-your-playlist"></a><span data-ttu-id="3461d-110">步骤1：为播放列表创建 SharePoint 页面</span><span class="sxs-lookup"><span data-stu-id="3461d-110">Step 1: Create a SharePoint page for your playlist</span></span>
<span data-ttu-id="3461d-111">在此示例中，我们将首先创建一个要添加到播放列表中的 SharePoint 页面。</span><span class="sxs-lookup"><span data-stu-id="3461d-111">In this example, we’ll first create a SharePoint page to add to the playlist.</span></span> <span data-ttu-id="3461d-112">我们将创建一个包含 YouTube 视频 web 部件和文本 web 部件的页面。</span><span class="sxs-lookup"><span data-stu-id="3461d-112">We’ll create a page with a YouTube video web part and Text web part.</span></span>  <span data-ttu-id="3461d-113">这些说明假定您使用的是 SharePoint Online 服务。</span><span class="sxs-lookup"><span data-stu-id="3461d-113">These instructions assume you are using the SharePoint Online service.</span></span> 

#### <a name="create-a-new-page"></a><span data-ttu-id="3461d-114">创建新页面</span><span class="sxs-lookup"><span data-stu-id="3461d-114">Create a new page</span></span>
1.  <span data-ttu-id="3461d-115">选择 "设置" 菜单，> 网站内容 > "网站页面 > 新的 > 网站" 页面。</span><span class="sxs-lookup"><span data-stu-id="3461d-115">Select the Settings menu > Site Contents > Site Pages > New > Site Page.</span></span>
2.  <span data-ttu-id="3461d-116">在 "标题" 区域中，键入 "使用团队" 命令框</span><span class="sxs-lookup"><span data-stu-id="3461d-116">In the title area, type Use the Teams command box</span></span>
3.  <span data-ttu-id="3461d-117">选择 "添加新内容" 部分，然后选择 "两列"。</span><span class="sxs-lookup"><span data-stu-id="3461d-117">Select the Add a new section, and then select Two Columns.</span></span>

![两列相加](media/clo365addtwocolumn.png)

4.  <span data-ttu-id="3461d-119">在左侧框中，选择 "添加新 web 部件"，然后选择 "嵌入"。</span><span class="sxs-lookup"><span data-stu-id="3461d-119">In the left-hand box, select Add a new web part, and then select Embed.</span></span> 
5.  <span data-ttu-id="3461d-120">在 Web 浏览器中，转到此 URL https://youtu.be/wYrRCRphrp0 并获取视频的嵌入代码。</span><span class="sxs-lookup"><span data-stu-id="3461d-120">In a Web browser, go to this URL https://youtu.be/wYrRCRphrp0 and get the embed code for the video.</span></span> 
6.  <span data-ttu-id="3461d-121">在 SharePoint Web 部件中，选择 "添加嵌入代码"，然后将其粘贴到 "嵌入" 框中。</span><span class="sxs-lookup"><span data-stu-id="3461d-121">In the SharePoint Web part, select Add Embed code and then paste it into the Embed box.</span></span> 
7.  <span data-ttu-id="3461d-122">在右侧的框中，选择 "添加新 web 部件"，然后选择 "文本"。</span><span class="sxs-lookup"><span data-stu-id="3461d-122">In the right-hand box, select Add a new web part, and then select Text.</span></span> 
8.  <span data-ttu-id="3461d-123">在 Web 浏览器中，转到此 URL： https://support.office.com/article/13c4e429-7324-4886-b377-5dbed539193b 并复制 Try！</span><span class="sxs-lookup"><span data-stu-id="3461d-123">In a Web browser, go to this URL: https://support.office.com/article/13c4e429-7324-4886-b377-5dbed539193b and copy the Try it!</span></span> <span data-ttu-id="3461d-124">页面中的说明，并将其粘贴到文本 Web 部件中。</span><span class="sxs-lookup"><span data-stu-id="3461d-124">Instructions from the page and paste them into the Text Web part.</span></span> <span data-ttu-id="3461d-125">页面应如下所示。</span><span class="sxs-lookup"><span data-stu-id="3461d-125">Your page should look like the following.</span></span> 

![嵌入页面](media/clo365teamscommandbox.png)

9.  <span data-ttu-id="3461d-127">单击 " **发布**"，然后复制页面的 URL 并将其粘贴到记事本中</span><span class="sxs-lookup"><span data-stu-id="3461d-127">Click **Publish**, and then copy the URL of the page and paste it in Notepad</span></span>

#### <a name="step-2-create-the-playlist"></a><span data-ttu-id="3461d-128">步骤2：创建播放列表</span><span class="sxs-lookup"><span data-stu-id="3461d-128">Step 2: Create the Playlist</span></span>

1. <span data-ttu-id="3461d-129">导航到网站体验中的 " **自定义学习管理** " 页。</span><span class="sxs-lookup"><span data-stu-id="3461d-129">Navigate to the **Custom Learning Administration** page in your site experience.</span></span>
<span data-ttu-id="3461d-130">![custom_admin.png](media/custom_admin.png)</span><span class="sxs-lookup"><span data-stu-id="3461d-130">![custom_admin.png](media/custom_admin.png)</span></span>
1. <span data-ttu-id="3461d-131">确保选择了 " **类别** "</span><span class="sxs-lookup"><span data-stu-id="3461d-131">Make sure **Category** is selected</span></span> 
1. <span data-ttu-id="3461d-132">单击要在其上显示新播放列表的类别</span><span class="sxs-lookup"><span data-stu-id="3461d-132">Click on the category where you'd like your new playlist to appear</span></span>
1. <span data-ttu-id="3461d-133">在 "类别名称" 旁边，单击加号符号 ![custom_addplay.png](media/custom_addplay.png)</span><span class="sxs-lookup"><span data-stu-id="3461d-133">Next to the category name, click on the plus symbol ![custom_addplay.png](media/custom_addplay.png)</span></span>

1. <span data-ttu-id="3461d-134">填写以下示例中所示的值，然后选择 " **创建**"。</span><span class="sxs-lookup"><span data-stu-id="3461d-134">Fill in the values as shown in the example below and select **Create**.</span></span> 
<span data-ttu-id="3461d-135">![custom_details.png](media/custom_details.png)</span><span class="sxs-lookup"><span data-stu-id="3461d-135">![custom_details.png](media/custom_details.png)</span></span>
- <span data-ttu-id="3461d-136">播放列表的**标题**-显示名称</span><span class="sxs-lookup"><span data-stu-id="3461d-136">**Title** - Display name of the playlist</span></span>
- <span data-ttu-id="3461d-137">**Description** -有关将学习的内容的信息</span><span class="sxs-lookup"><span data-stu-id="3461d-137">**Description** - Information about what will be learned</span></span>
- <span data-ttu-id="3461d-138">**类别** -根据初始选择预先选择</span><span class="sxs-lookup"><span data-stu-id="3461d-138">**Category** - Preselected based on your initial selection</span></span>
- <span data-ttu-id="3461d-139">**子类别** -根据您的初始选择预选</span><span class="sxs-lookup"><span data-stu-id="3461d-139">**Sub Category** - Preselected based on your intial selection</span></span>
- <span data-ttu-id="3461d-140">**技术** -选择 "适用"</span><span class="sxs-lookup"><span data-stu-id="3461d-140">**Technology** - Select as applicable</span></span>
- <span data-ttu-id="3461d-141">**Level** -初级、Intermidate 或 Advanced</span><span class="sxs-lookup"><span data-stu-id="3461d-141">**Level** - Beginner, Intermidate or Advanced</span></span>
- <span data-ttu-id="3461d-142">**受众** -这使您可以根据 Microsoft 提供的预定义角色的列表来设定内容目标。</span><span class="sxs-lookup"><span data-stu-id="3461d-142">**Audience** - This allows you to target content based on a pre-defined list of roles provided by Microsoft.</span></span>

6. <span data-ttu-id="3461d-143">单击 "**保存详细信息**"</span><span class="sxs-lookup"><span data-stu-id="3461d-143">Click **Save Detail**</span></span>

> [!TIP]
> <span data-ttu-id="3461d-144">您可以自定义播放列表图标图像。</span><span class="sxs-lookup"><span data-stu-id="3461d-144">You can customize the icon image for your playlist.</span></span>  <span data-ttu-id="3461d-145">单击图像图标并插入之前上载的图像的 URL。</span><span class="sxs-lookup"><span data-stu-id="3461d-145">Click the image icon and insert an URL of a previously uploaded image.</span></span>  <span data-ttu-id="3461d-146">请确保该图像位于自定义学习网站集内，或者位于其他所有用户都有权访问该文件的位置。</span><span class="sxs-lookup"><span data-stu-id="3461d-146">Make sure the image is located within the Custom Learning site collection or in another location that all users will have access to the file.</span></span>  
<span data-ttu-id="3461d-147">![custom_image.png](media/custom_image.png)</span><span class="sxs-lookup"><span data-stu-id="3461d-147">![custom_image.png](media/custom_image.png)</span></span>

#### <a name="step-3-add-assets-to-the-playlist"></a><span data-ttu-id="3461d-148">步骤3：将资产添加到播放列表</span><span class="sxs-lookup"><span data-stu-id="3461d-148">Step 3: Add assets to the playlist</span></span>
<span data-ttu-id="3461d-149">在此步骤中，您将向播放列表中添加来自 Microsoft 和您创建的 SharePoint 页面的现有资产。</span><span class="sxs-lookup"><span data-stu-id="3461d-149">In this step, you’ll add existing assets from Microsoft and the SharePoint page you created to the playlist.</span></span> 

1. <span data-ttu-id="3461d-150">保存了播放列表的详细信息后，便可使用搜索现有资产。</span><span class="sxs-lookup"><span data-stu-id="3461d-150">Once you have saved the details for your Playlist you can use the Search for Existing Assets.</span></span>
1. <span data-ttu-id="3461d-151">**在任何搜索词中输入** ，以查看其他播放列表中提供的预定义资产的列表。</span><span class="sxs-lookup"><span data-stu-id="3461d-151">**Enter in any search term** to see a list of predefined assets that are available from other playlists.</span></span> <span data-ttu-id="3461d-152">**单击** 资产的名称以将其包含在新的播放列表中。</span><span class="sxs-lookup"><span data-stu-id="3461d-152">**Click on the name** of an asset to include it in your new playlist.</span></span>
<span data-ttu-id="3461d-153">![custom_slist.png](media/custom_slist.png)</span><span class="sxs-lookup"><span data-stu-id="3461d-153">![custom_slist.png](media/custom_slist.png)</span></span>

<span data-ttu-id="3461d-154">您还可以添加之前创建的 SharePoint 页面，也可以在体验中从头开始创建它。</span><span class="sxs-lookup"><span data-stu-id="3461d-154">You can also add the SharePoint page you created earlier or create one from scratch in the experience.</span></span>

1. <span data-ttu-id="3461d-155">单击 "播放列表资产" 对话框中的 " **新建资产** " 选项</span><span class="sxs-lookup"><span data-stu-id="3461d-155">Click on the **New Asset** option in the Playlist Assets dialog</span></span>
1. <span data-ttu-id="3461d-156">为您的资产提供 **标题**。</span><span class="sxs-lookup"><span data-stu-id="3461d-156">Give your asset a **Title**.</span></span> <span data-ttu-id="3461d-157">输入后，其他选项将显示 ![custom_newpage.png](media/custom_newpage.png)</span><span class="sxs-lookup"><span data-stu-id="3461d-157">Once entered, additional options will display ![custom_newpage.png](media/custom_newpage.png)</span></span>
1. <span data-ttu-id="3461d-158">您现在可以在 SharePoint Online 中创建新的资产页面，也可以在现有页面的 URL 中输入以将其添加到自定义播放列表中。</span><span class="sxs-lookup"><span data-stu-id="3461d-158">You can now create a new asset page in SharePoint Online or enter in the URL of an existing page to add it to your custom playlist.</span></span> 
1. <span data-ttu-id="3461d-159">"**类别**"、"**子类别**" 和 "**技术**" 字段将根据您以前的选择，为此播放列表预先填充。</span><span class="sxs-lookup"><span data-stu-id="3461d-159">**Category**, **Sub Category** and **Technology** fields will be pre-populated based on your previous selections for this playlist.</span></span>
1. <span data-ttu-id="3461d-160">为此单个资产的级别和受众做出适当的选择。</span><span class="sxs-lookup"><span data-stu-id="3461d-160">Make the appropriate selections for Level and Audience for this individual asset.</span></span>  
1. <span data-ttu-id="3461d-161">单击 " **保存资产** " 以将其添加到自定义播放列表</span><span class="sxs-lookup"><span data-stu-id="3461d-161">Click **Save Asset** to add it to the custom playlist</span></span>
1. <span data-ttu-id="3461d-162">重复这些步骤，可以搜索或添加单个页面，直到完成播放列表。</span><span class="sxs-lookup"><span data-stu-id="3461d-162">Repeat these steps, either searching or adding individual pages, until your playlist is complete.</span></span> 
1. <span data-ttu-id="3461d-163">单击 " **关闭播放列表** " 以保存</span><span class="sxs-lookup"><span data-stu-id="3461d-163">Click **Close Playlist** to save</span></span>

<span data-ttu-id="3461d-164">包含此内容的播放列表现在将在你已安装/嵌入自定义学习 web 部件的任何位置可用。</span><span class="sxs-lookup"><span data-stu-id="3461d-164">Your playlist with this content will now be available anywhere you have installed / embedded the Custom Learning webpart.</span></span> 

> [!NOTE]
> <span data-ttu-id="3461d-165">如果您在关闭播放列表后出错了，可以通过单击播放列表名称旁边的 X 将其从类别中删除。</span><span class="sxs-lookup"><span data-stu-id="3461d-165">If you make a mistake once you have closed the playlist, you can delete it from the category by clicking the X next to the playlist name.</span></span>  

#### <a name="things-to-think-about"></a><span data-ttu-id="3461d-166">要考虑的事项</span><span class="sxs-lookup"><span data-stu-id="3461d-166">Things to Think About</span></span>

<span data-ttu-id="3461d-167">自定义播放列表可用于帮助最终用户完成各种任务。</span><span class="sxs-lookup"><span data-stu-id="3461d-167">Custom playlists can be used to assist your end users in a variety of tasks.</span></span>  <span data-ttu-id="3461d-168">您是否有时间请求窗体？</span><span class="sxs-lookup"><span data-stu-id="3461d-168">Do you have a time off request form?</span></span>  <span data-ttu-id="3461d-169">请求硬件设备的表单？</span><span class="sxs-lookup"><span data-stu-id="3461d-169">A form to request hardware equipment?</span></span>  <span data-ttu-id="3461d-170">可以将任何现有的培训资产编程到体验中。</span><span class="sxs-lookup"><span data-stu-id="3461d-170">Any existing training assets can be programmed into the experience.</span></span>  

## <a name="share-playlists"></a><span data-ttu-id="3461d-171">共享播放列表</span><span class="sxs-lookup"><span data-stu-id="3461d-171">Share Playlists</span></span>

1. <span data-ttu-id="3461d-172">导航到 web 部件或网站体验中的任何播放列表</span><span class="sxs-lookup"><span data-stu-id="3461d-172">Navigate to any playlist within the webpart or site experience</span></span>
1. <span data-ttu-id="3461d-173">在左上角，将看到三个图标</span><span class="sxs-lookup"><span data-stu-id="3461d-173">In the upper left hand corner you will see three icons</span></span>
1. <span data-ttu-id="3461d-174">单击代表链接的图标</span><span class="sxs-lookup"><span data-stu-id="3461d-174">Click on the icon representing a link</span></span>
1. <span data-ttu-id="3461d-175">将 URL 复制到播放列表</span><span class="sxs-lookup"><span data-stu-id="3461d-175">Copy the URL to the playlist</span></span>

<span data-ttu-id="3461d-176">![share.png](media/share.png) 现在可以在网站导航中插入或在其他通信中使用此 URL，以将员工直接转到该播放列表。</span><span class="sxs-lookup"><span data-stu-id="3461d-176">![share.png](media/share.png) This URL can now be inserted in your site navigation or utilized in other communications to take your employees directly to that playlist.</span></span> 

### <a name="next-steps---drive-adoption"></a><span data-ttu-id="3461d-177">后续步骤- [驱动器采用](driveadoption.md)</span><span class="sxs-lookup"><span data-stu-id="3461d-177">Next Steps - [Drive Adoption](driveadoption.md)</span></span>
