---
author: pkrebs
ms.author: pkrebs
title: 为播放列表创建 SharePoint 页面
ms.date: 02/10/2019
description: 为播放列表创建 SharePoint 页面
ms.openlocfilehash: c2de66a0746260e8f6539656ad70052b209c54ba
ms.sourcegitcommit: e10085e60ca3f38029fde229fb093e6bc4a34203
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/19/2019
ms.locfileid: "30103687"
---
# <a name="create-sharepoint-pages-for-custom-playlists"></a><span data-ttu-id="f4bb6-103">为自定义播放列表创建 SharePoint 页面</span><span class="sxs-lookup"><span data-stu-id="f4bb6-103">Create SharePoint pages for Custom Playlists</span></span>

<span data-ttu-id="f4bb6-p101">自定义学习的独特功能之一是能够创建从 Microsoft 的资产和您创建的 SharePoint 资产汇编的播放列表。在此示例中, 我们将事先创建一个 SharePoint 页来创建播放列表。通过 SharePoint 页面构建播放列表的功能可提供多种机会, 以使用 Microsoft 或你的组织提供的 Web 部件构建页面。例如, 播放列表可以包括 SharePoint 页面, 其中包含来自 YouTube 的嵌入式视频, 或从 Office 365 表单或嵌入的 Power BI 报表生成的表单。在此示例中, 我们将介绍如何使用 "嵌入 web 部件" 和 "文本" web 部件生成页面。</span><span class="sxs-lookup"><span data-stu-id="f4bb6-p101">One of the unique features of Custom Learning is the ability to create playlists that are assembled from assets from Microsoft and from SharePoint assets that you create. In this example, we’ll create a SharePoint page in advance of creating a playlist. The ability to build playlists from SharePoint pages offers a variety of opportunities to build pages using the Web parts available from Microsoft or your organization. For example, a playlist can include a SharePoint page with embedded videos from YouTube, or a form built from Office 365 Forms, or an embedded Power BI report. In this example, we’ll show you how to build a page with the Embed web part and the Text web part.</span></span>  

## <a name="create-a-sharepoint-page-for-a-custom-playlist"></a><span data-ttu-id="f4bb6-109">为自定义播放列表创建 SharePoint 页面</span><span class="sxs-lookup"><span data-stu-id="f4bb6-109">Create a SharePoint page for a custom playlist</span></span>

1. <span data-ttu-id="f4bb6-110">单击 "SharePoint**齿轮**" 图标, 然后单击 "**添加页面**"。</span><span class="sxs-lookup"><span data-stu-id="f4bb6-110">Click the SharePoint **Gear** icon, and then click **Add a page**.</span></span>
2. <span data-ttu-id="f4bb6-111">单击页面左侧的 "**添加新分区 (+)** ", 然后单击 "**两栏**" 以查看分区布局。</span><span class="sxs-lookup"><span data-stu-id="f4bb6-111">Click **Add a new section (+)** on the left-hand side of the page, and then click **Two Columns** for the section layout.</span></span>
3. <span data-ttu-id="f4bb6-112">在左侧列中, 单击 "+", 然后单击 "**嵌入**web 部件"。</span><span class="sxs-lookup"><span data-stu-id="f4bb6-112">In the left column, click + , and then click the **Embed** web part.</span></span> 
4. <span data-ttu-id="f4bb6-p102">在右列中, 单击 "+", 然后单击 "**文本**" web 部件。页面应如下所示。</span><span class="sxs-lookup"><span data-stu-id="f4bb6-p102">In the right column, click +, and then click the **Text** web part. Your page should look like this.</span></span>

![cg-pagenewstart](media/cg-pagenewstart.png)

### <a name="add-a-video-and-text-from-youtube"></a><span data-ttu-id="f4bb6-116">从 YouTube 添加视频和文本</span><span class="sxs-lookup"><span data-stu-id="f4bb6-116">Add a video and text from YouTube</span></span>

1. <span data-ttu-id="f4bb6-p103">在浏览器中, 转到 "YouTube"。对于此示例, 请搜索 "什么是 Office 365 – Microsoft 的最佳生产力应用程序"。</span><span class="sxs-lookup"><span data-stu-id="f4bb6-p103">In your browser, go to YouTube. For this example, search for “What is Office 365 – Microsoft’s best productivity apps”.</span></span>
2. <span data-ttu-id="f4bb6-119">单击视频进行播放, 然后将其暂停, 然后右键单击该视频。</span><span class="sxs-lookup"><span data-stu-id="f4bb6-119">Click the video to play it, then pause it, then right-click on it.</span></span> 
3. <span data-ttu-id="f4bb6-120">单击 "**复制嵌入代码**", 然后返回到 "SharePoint" 页面。</span><span class="sxs-lookup"><span data-stu-id="f4bb6-120">Click **Copy embed code**, then return to the SharePoint page.</span></span> 
4. <span data-ttu-id="f4bb6-121">单击 "**嵌入**web 部件" 中的 "**添加嵌入代码**", 然后添加 YouTube 视频中的代码。</span><span class="sxs-lookup"><span data-stu-id="f4bb6-121">Click **Add embed code** in the **Embed** web part, and then add the code from the YouTube video.</span></span>
5. <span data-ttu-id="f4bb6-122">返回到 YouTube 页面, 并复制视频的**说明**文本。</span><span class="sxs-lookup"><span data-stu-id="f4bb6-122">Return to the YouTube page and copy the **Description** text for the video.</span></span> 
6. <span data-ttu-id="f4bb6-123">返回到 "SharePoint" 页面, 选择 "**文本**" web 部件, 然后复制 YouTube 视频中的文本。</span><span class="sxs-lookup"><span data-stu-id="f4bb6-123">Return to the SharePoint page, select the **Text** web part, then copy the text from the YouTube video.</span></span>
7. <span data-ttu-id="f4bb6-124">在 SharePoint 页面的 "标题" 区域中选择 "**编辑 web 部件**" 图标, 然后将该页面命名为 "自定义播放列表简介"。</span><span class="sxs-lookup"><span data-stu-id="f4bb6-124">Select the **Edit web part** icon  in the Title area of the SharePoint page, and then name the page “Custom Playlist Introduction”.</span></span> 
8. <span data-ttu-id="f4bb6-p104">对于 "**布局**", 选择 "**无**", 然后关闭 "**标题区域**属性" 窗格。此时, 页面应类似于以下内容。</span><span class="sxs-lookup"><span data-stu-id="f4bb6-p104">For **Layout**, select **Plain**, then close **Title Region** properties pane. The page should now look something like the following.</span></span> 

![cg-pagenewfinish](media/cg-pagenewfinish.png)

### <a name="publish-the-page"></a><span data-ttu-id="f4bb6-128">发布页面</span><span class="sxs-lookup"><span data-stu-id="f4bb6-128">Publish the page</span></span>

- <span data-ttu-id="f4bb6-p105">选择 "**发布**" 按钮。现在, 你已准备好将此 SharePoint 页面添加到自定义播放列表中。</span><span class="sxs-lookup"><span data-stu-id="f4bb6-p105">Select the **Publish** button. Now you're ready to add this SharePoint page to your custom playlist.</span></span> 