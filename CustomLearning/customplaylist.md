# <a name="customize-the-services-and-playlists"></a><span data-ttu-id="c8d4d-101">自定义的服务和播放列表</span><span class="sxs-lookup"><span data-stu-id="c8d4d-101">Customize the Services and Playlists</span></span>

<span data-ttu-id="c8d4d-p101">默认情况下的网站体验和 web 部件包含的所有 Office 365 服务的内容。 如果只全部或部分这些服务可在贵公司可以调整内容可供您的用户。 在本文中，我们将自定义 web 部件内容。</span><span class="sxs-lookup"><span data-stu-id="c8d4d-p101">By default both the site experience and the webpart include content for all Office 365 services.  If only all or some of these services are available in your company you can adjust what content is available to your users.  In this article we will customize the webpart content.</span></span>  

## <a name="customizing-the-webpart-content"></a><span data-ttu-id="c8d4d-105">自定义 web 部件内容</span><span class="sxs-lookup"><span data-stu-id="c8d4d-105">Customizing the webpart content</span></span>

<span data-ttu-id="c8d4d-106">自定义学习 web 部件提供了两个主要功能：</span><span class="sxs-lookup"><span data-stu-id="c8d4d-106">The Custom Learning webpart provides two key features:</span></span>
- <span data-ttu-id="c8d4d-107">隐藏/显示技术</span><span class="sxs-lookup"><span data-stu-id="c8d4d-107">Hide/Show Technologies</span></span>
- <span data-ttu-id="c8d4d-108">创建播放列表</span><span class="sxs-lookup"><span data-stu-id="c8d4d-108">Create a Playlist</span></span>

### <a name="hide-or-show-technology-categories"></a><span data-ttu-id="c8d4d-109">隐藏或显示技术类别</span><span class="sxs-lookup"><span data-stu-id="c8d4d-109">Hide or Show Technology Categories</span></span>

<span data-ttu-id="c8d4d-110">若要隐藏和显示 Web 部件的内容：</span><span class="sxs-lookup"><span data-stu-id="c8d4d-110">To hide and show content in the Web part:</span></span> 
1.  <span data-ttu-id="c8d4d-111">单击下拉菜单上 web 部件，然后单击隐藏/显示技术</span><span class="sxs-lookup"><span data-stu-id="c8d4d-111">Click the dropdown menu on the webpart, then click Hide/Show Technologies</span></span>

![菜单选项](media/clohideshow.png)

2. <span data-ttu-id="c8d4d-113">选择 checkox 为隐藏或显示技术并选择**应用**。</span><span class="sxs-lookup"><span data-stu-id="c8d4d-113">Select a checkox to hide or show a technology and select **Apply**.</span></span>

![技术选项](media/clohideshow1.png)

### <a name="create-a-playlist"></a><span data-ttu-id="c8d4d-115">创建播放列表</span><span class="sxs-lookup"><span data-stu-id="c8d4d-115">Create a Playlist</span></span>

<span data-ttu-id="c8d4d-p102">播放列表是"资产"compliation。"资源"是一个 SharePoint 页面或现有的 Microsoft 培训内容项。创建播放列表时您选择在一起的资产创建用户学习路径。</span><span class="sxs-lookup"><span data-stu-id="c8d4d-p102">A playlist is a compliation of "assets". An "asset" is a SharePoint page or existing item of Microsoft training content. When you create a playlist you select assets that go together to create a learning path for your user.</span></span>  

<span data-ttu-id="c8d4d-p103">添加 SharePoint 页的好处是，您可以创建 SharePoint 页面与 YouTube 视频或承载您的组织中的视频。您还可以使用窗体或其他 Office 365 内容创建页面。</span><span class="sxs-lookup"><span data-stu-id="c8d4d-p103">The benefit of adding SharePoint pages is that you can create SharePoint pages with a YouTube videos or videos hosted in your organization. You can also create pages with Forms or other Office 365 content.</span></span>  

#### <a name="step-1-create-a-sharepoint-page-for-your-playlist"></a><span data-ttu-id="c8d4d-121">步骤 1： 创建用于播放列表的 SharePoint 页面</span><span class="sxs-lookup"><span data-stu-id="c8d4d-121">Step 1: Create a SharePoint page for your playlist</span></span>
<span data-ttu-id="c8d4d-p104">本示例中，我们将首先创建 SharePoint 页添加到播放列表。我们将创建具有 YouTube 视频的 web 部件和文本 web 部件的页面。 这些说明假定您使用 SharePoint Online 服务。</span><span class="sxs-lookup"><span data-stu-id="c8d4d-p104">In this example, we’ll first create a SharePoint page to add to the playlist. We’ll create a page with a YouTube video web part and Text web part.  These instructions assume you are using the SharePoint Online service.</span></span> 

#### <a name="create-a-new-page"></a><span data-ttu-id="c8d4d-125">创建新的页面</span><span class="sxs-lookup"><span data-stu-id="c8d4d-125">Create a new page</span></span>
1.  <span data-ttu-id="c8d4d-126">选择设置菜单 > 网站内容 > 网站页面 > 新 > 网页。</span><span class="sxs-lookup"><span data-stu-id="c8d4d-126">Select the Settings menu > Site Contents > Site Pages > New > Site Page.</span></span>
2.  <span data-ttu-id="c8d4d-127">在标题区域中，键入使用团队命令框</span><span class="sxs-lookup"><span data-stu-id="c8d4d-127">In the title area, type Use the Teams command box</span></span>
3.  <span data-ttu-id="c8d4d-128">选择添加新的部分，然后选择两列。</span><span class="sxs-lookup"><span data-stu-id="c8d4d-128">Select the Add a new section, and then select Two Columns.</span></span>

![两列添加](media/clo365addtwocolumn.png)

4.  <span data-ttu-id="c8d4d-130">在左侧的框中，选择添加新的 web 部件，然后选择嵌入。</span><span class="sxs-lookup"><span data-stu-id="c8d4d-130">In the left-hand box, select Add a new web part, and then select Embed.</span></span> 
5.  <span data-ttu-id="c8d4d-131">在 Web 浏览器中，转到此 URLhttps://youtu.be/wYrRCRphrp0和获取视频嵌入代码。</span><span class="sxs-lookup"><span data-stu-id="c8d4d-131">In a Web browser, go to this URL https://youtu.be/wYrRCRphrp0 and get the embed code for the video.</span></span> 
6.  <span data-ttu-id="c8d4d-132">在 SharePoint Web 部件中，选择添加嵌入代码，然后将其粘贴到嵌入框中。</span><span class="sxs-lookup"><span data-stu-id="c8d4d-132">In the SharePoint Web part, select Add Embed code and then paste it into the Embed box.</span></span> 
7.  <span data-ttu-id="c8d4d-133">在右侧的框中，选择添加新的 web 部件，然后选择文本。</span><span class="sxs-lookup"><span data-stu-id="c8d4d-133">In the right-hand box, select Add a new web part, and then select Text.</span></span> 
8.  <span data-ttu-id="c8d4d-p105">在 Web 浏览器中，转到此 URL: https://support.office.com/en-us/article/13c4e429-7324-4886-b377-5dbed539193b ，并将复制 Try 它 ！从页上的说明并将它们粘贴到文本 Web 部件。网页应如下所示。</span><span class="sxs-lookup"><span data-stu-id="c8d4d-p105">In a Web browser, go to this URL: https://support.office.com/en-us/article/13c4e429-7324-4886-b377-5dbed539193b and copy the Try it! Instructions from the page and paste them into the Text Web part. Your page should look like the following.</span></span> 

![嵌入页](media/clo365teamscommandbox.png)

9.  <span data-ttu-id="c8d4d-138">单击发布，然后将复制的页面的 URL 并将其粘贴到记事本中</span><span class="sxs-lookup"><span data-stu-id="c8d4d-138">Click Publish, and then copy the URL of the page and paste it in Notepad</span></span>

#### <a name="step-2-create-the-playlist"></a><span data-ttu-id="c8d4d-139">步骤 2： 创建播放列表</span><span class="sxs-lookup"><span data-stu-id="c8d4d-139">Step 2: Create the Playlist</span></span>
1.  <span data-ttu-id="c8d4d-p106">导航到您安装自定义学习 web 部件。网站的完整体验它位于上的 Office 365 培训页面。</span><span class="sxs-lookup"><span data-stu-id="c8d4d-p106">Navigate to where you have installed the Custom Learning webpart. In the full site experience it is hosted on the Office 365 training page.</span></span> 
2.  <span data-ttu-id="c8d4d-142">从下拉菜单中选择创建新的播放列表。</span><span class="sxs-lookup"><span data-stu-id="c8d4d-142">From the dropdown menu select Create New Playlist.</span></span> 

![创建自定义播放列表](media/clo365createplaylist.png)

3.  <span data-ttu-id="c8d4d-144">下面的示例中所示填充的值，然后选择**创建**。</span><span class="sxs-lookup"><span data-stu-id="c8d4d-144">Fill in the values as shown in the example below and select **Create**.</span></span> 

#### <a name="step-3-add-assets-to-the-playlist"></a><span data-ttu-id="c8d4d-145">步骤 3： 将资源添加到播放列表</span><span class="sxs-lookup"><span data-stu-id="c8d4d-145">Step 3: Add assets to the playlist</span></span>
<span data-ttu-id="c8d4d-146">此步骤中，将从 Microsoft 和创建的 SharePoint 页中将现有资源添加到播放列表中。</span><span class="sxs-lookup"><span data-stu-id="c8d4d-146">In this step, you’ll add existing assets from Microsoft and the SharePoint page you created to the playlist.</span></span> 

1.  <span data-ttu-id="c8d4d-147">单击菜单按钮，然后单击添加现有资产。</span><span class="sxs-lookup"><span data-stu-id="c8d4d-147">Click the menu button, then click Add Existing Asset.</span></span>

![添加资源](media/clo365addasset.png)

2.  <span data-ttu-id="c8d4d-149">筛选上的 Office 365 应用程序 > Microsoft 团队培训</span><span class="sxs-lookup"><span data-stu-id="c8d4d-149">Filter on Office 365 Apps > Microsoft Teams Training</span></span>
3.  <span data-ttu-id="c8d4d-150">欢迎使用添加 Microsoft 团队、 启动并正在运行，获取您的团队和启动聊天和发起呼叫。</span><span class="sxs-lookup"><span data-stu-id="c8d4d-150">Add Welcome to Microsoft Teams, Get your team up and running, and Start chats and make calls.</span></span>
4.  <span data-ttu-id="c8d4d-151">选择菜单按钮 > 创建资产。</span><span class="sxs-lookup"><span data-stu-id="c8d4d-151">Select the menu button > Create Asset.</span></span>
5.  <span data-ttu-id="c8d4d-152">资产标题框中，使用团队命令框类型。</span><span class="sxs-lookup"><span data-stu-id="c8d4d-152">Type Use the Teams command box in the Asset title box.</span></span> 
6.  <span data-ttu-id="c8d4d-153">粘贴 SharePoint 使用的资产的内容字段中复制的团队命令框页面 URL。</span><span class="sxs-lookup"><span data-stu-id="c8d4d-153">Paste the SharePoint Use the Teams command box page URL you copied in the Asset content field.</span></span> 
7.  <span data-ttu-id="c8d4d-p107">现在导航回主页 > 自定义播放列表 > 您第一天团队 > 与使用团队命令框。网页应如下所示。</span><span class="sxs-lookup"><span data-stu-id="c8d4d-p107">Now navigate back to the Home Page > Custom Playlists > Your first days with Teams > Use the Teams command box. Your page should look like the following.</span></span> 

![创建的页面](media/clo365createplaylist2.png)

<span data-ttu-id="c8d4d-157">与此内容播放列表现在将可用无处不在已安装 / 嵌入自定义学习 web 部件。</span><span class="sxs-lookup"><span data-stu-id="c8d4d-157">Your playlist with this content will now be available anywhere you have installed / embedded the Custom Learning webpart.</span></span> 

#### <a name="things-to-think-about"></a><span data-ttu-id="c8d4d-158">要考虑的事项</span><span class="sxs-lookup"><span data-stu-id="c8d4d-158">Things to Think About</span></span>

<span data-ttu-id="c8d4d-p108">自定义播放列表可用于帮助您的最终用户任务 vareity。 您必须关闭请求表单的时间？ 表单请求硬件设备？ 任何现有的培训资产可以编入体验。</span><span class="sxs-lookup"><span data-stu-id="c8d4d-p108">Custom playlists can be used to assist your end users in a vareity of tasks.  Do you have a time off request form?  A form to request hardware equipment?  Any existing training assets can be programmed into the experience.</span></span>  
