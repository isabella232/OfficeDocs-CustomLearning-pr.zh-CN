---
author: pkrebs
ms.author: pkrebs
title: 为SharePoint创建页面
ms.date: 02/10/2019
description: 为SharePoint创建页面
ms.service: sharepoint-online
manager: bpardi
ms.topic: article
ms.openlocfilehash: ce4a204b3072469840b6f3fa8f93d9e78833b181
ms.sourcegitcommit: 956ab22dd8ce23ee1779f1a01d34b434243c3cb1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2021
ms.locfileid: "52310656"
---
# <a name="create-sharepoint-pages-for-custom-playlists"></a><span data-ttu-id="ce0bb-103">为SharePoint播放列表创建页面</span><span class="sxs-lookup"><span data-stu-id="ce0bb-103">Create SharePoint pages for Custom Playlists</span></span>

<span data-ttu-id="ce0bb-104">学习路径的独特功能之一是，能够创建从 Microsoft 资产和所创建资产SharePoint集合的播放列表。</span><span class="sxs-lookup"><span data-stu-id="ce0bb-104">One of the unique features of learning pathways is the ability to create playlists that are assembled from assets from Microsoft and from SharePoint assets that you create.</span></span> <span data-ttu-id="ce0bb-105">本示例中，我们将先创建一个SharePoint页面，然后创建播放列表。</span><span class="sxs-lookup"><span data-stu-id="ce0bb-105">In this example, we’ll create a SharePoint page in advance of creating a playlist.</span></span> <span data-ttu-id="ce0bb-106">从页面生成播放列表SharePoint提供了使用 Microsoft 或组织提供的 Web 部件生成页面的各种机会。</span><span class="sxs-lookup"><span data-stu-id="ce0bb-106">The ability to build playlists from SharePoint pages offers a variety of opportunities to build pages using the Web parts available from Microsoft or your organization.</span></span> <span data-ttu-id="ce0bb-107">例如，播放列表可以包括一个SharePoint YouTube 中的嵌入式视频的页面、一个从 Office 365 Forms 构建的表单或一个嵌入式 Power BI 报表。</span><span class="sxs-lookup"><span data-stu-id="ce0bb-107">For example, a playlist can include a SharePoint page with embedded videos from YouTube, or a form built from Office 365 Forms, or an embedded Power BI report.</span></span> <span data-ttu-id="ce0bb-108">本示例将展示如何使用嵌入 Web 部件和文本 Web 部件生成页面。</span><span class="sxs-lookup"><span data-stu-id="ce0bb-108">In this example, we’ll show you how to build a page with the Embed web part and the Text web part.</span></span>  

## <a name="create-a-sharepoint-page-for-a-custom-playlist"></a><span data-ttu-id="ce0bb-109">为自定义SharePoint创建一个自定义播放列表页面</span><span class="sxs-lookup"><span data-stu-id="ce0bb-109">Create a SharePoint page for a custom playlist</span></span>

1. <span data-ttu-id="ce0bb-110">单击"SharePoint **齿轮"图标**，然后单击"**添加页面"。**</span><span class="sxs-lookup"><span data-stu-id="ce0bb-110">Click the SharePoint **Gear** icon, and then click **Add a page**.</span></span>
2. <span data-ttu-id="ce0bb-111">单击 **页面左侧的**" (+) "，然后单击"两列"作为该节布局。 </span><span class="sxs-lookup"><span data-stu-id="ce0bb-111">Click **Add a new section (+)** on the left-hand side of the page, and then click **Two Columns** for the section layout.</span></span>
3. <span data-ttu-id="ce0bb-112">在左侧列中，单击"+"，然后单击" **嵌入** Web 部件"。</span><span class="sxs-lookup"><span data-stu-id="ce0bb-112">In the left column, click + , and then click the **Embed** web part.</span></span> 
4. <span data-ttu-id="ce0bb-113">在右侧列中，单击"+"，然后单击"文本 **"Web** 部件。</span><span class="sxs-lookup"><span data-stu-id="ce0bb-113">In the right column, click +, and then click the **Text** web part.</span></span> <span data-ttu-id="ce0bb-114">你的页面应如下所示。</span><span class="sxs-lookup"><span data-stu-id="ce0bb-114">Your page should look like this.</span></span>

![cg-pagenewstart.png](media/cg-pagenewstart.png)

### <a name="add-a-video-and-text-from-youtube"></a><span data-ttu-id="ce0bb-116">从 YouTube 添加视频和文本</span><span class="sxs-lookup"><span data-stu-id="ce0bb-116">Add a video and text from YouTube</span></span>

1. <span data-ttu-id="ce0bb-117">在浏览器中，转到 YouTube。</span><span class="sxs-lookup"><span data-stu-id="ce0bb-117">In your browser, go to YouTube.</span></span> <span data-ttu-id="ce0bb-118">对于此示例，搜索"什么是Office 365 – Microsoft 的最佳生产力应用"。</span><span class="sxs-lookup"><span data-stu-id="ce0bb-118">For this example, search for “What is Office 365 – Microsoft’s best productivity apps”.</span></span>
2. <span data-ttu-id="ce0bb-119">单击视频以播放它，然后暂停它，然后右键单击它。</span><span class="sxs-lookup"><span data-stu-id="ce0bb-119">Click the video to play it, then pause it, then right-click on it.</span></span> 
3. <span data-ttu-id="ce0bb-120">单击 **"复制嵌入代码**"，然后返回到SharePoint页。</span><span class="sxs-lookup"><span data-stu-id="ce0bb-120">Click **Copy embed code**, then return to the SharePoint page.</span></span> 
4. <span data-ttu-id="ce0bb-121">单击 **"在嵌入** Web **部件中添加** 嵌入代码"，然后从 YouTube 视频添加代码。</span><span class="sxs-lookup"><span data-stu-id="ce0bb-121">Click **Add embed code** in the **Embed** web part, and then add the code from the YouTube video.</span></span>
5. <span data-ttu-id="ce0bb-122">返回到 YouTube 页面并复制 **视频的说明** 文本。</span><span class="sxs-lookup"><span data-stu-id="ce0bb-122">Return to the YouTube page and copy the **Description** text for the video.</span></span> 
6. <span data-ttu-id="ce0bb-123">返回到"SharePoint"页，选择"**文本**"Web 部件，然后从 YouTube 视频复制文本。</span><span class="sxs-lookup"><span data-stu-id="ce0bb-123">Return to the SharePoint page, select the **Text** web part, then copy the text from the YouTube video.</span></span>
7. <span data-ttu-id="ce0bb-124">选择页面标题 **区域中** 的"编辑 Web SharePoint图标，然后将页面命名为"自定义播放列表简介"。</span><span class="sxs-lookup"><span data-stu-id="ce0bb-124">Select the **Edit web part** icon  in the Title area of the SharePoint page, and then name the page “Custom Playlist Introduction”.</span></span> 
8. <span data-ttu-id="ce0bb-125">对于 **"布局"，\*\*\*\*选择"纯**"，然后关闭 **"标题区域** 属性"窗格。</span><span class="sxs-lookup"><span data-stu-id="ce0bb-125">For **Layout**, select **Plain**, then close **Title Region** properties pane.</span></span> <span data-ttu-id="ce0bb-126">现在，页面应如下所示。</span><span class="sxs-lookup"><span data-stu-id="ce0bb-126">The page should now look something like the following.</span></span> 

![cg-pagenewfinish.png](media/cg-pagenewfinish.png)

### <a name="publish-the-page"></a><span data-ttu-id="ce0bb-128">发布页面</span><span class="sxs-lookup"><span data-stu-id="ce0bb-128">Publish the page</span></span>

- <span data-ttu-id="ce0bb-129">选择" **发布"** 按钮。</span><span class="sxs-lookup"><span data-stu-id="ce0bb-129">Select the **Publish** button.</span></span> <span data-ttu-id="ce0bb-130">现在，你已准备好将此SharePoint添加到你的自定义播放列表。</span><span class="sxs-lookup"><span data-stu-id="ce0bb-130">Now you're ready to add this SharePoint page to your custom playlist.</span></span> 