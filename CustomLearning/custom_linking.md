---
author: pkrebs
ms.author: pkrebs
title: 链接到自定义学习资产
ms.date: 02/15/2019
description: 如何链接到自定义学习资产
ms.openlocfilehash: cdde37f370663ca50241833a15e8411921b45a1b
ms.sourcegitcommit: 775d6807291ab263eea5ec649d9aaf1933fb41ca
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/23/2019
ms.locfileid: "32056141"
---
# <a name="link-to-custom-learning-content"></a><span data-ttu-id="37bf0-103">指向自定义学习内容的链接</span><span class="sxs-lookup"><span data-stu-id="37bf0-103">Link to Custom Learning content</span></span>

<span data-ttu-id="37bf0-104">通过自定义学习, 有两种方法可链接到内容:</span><span class="sxs-lookup"><span data-stu-id="37bf0-104">With Custom Learning, there are two ways to link to content:</span></span>

- <span data-ttu-id="37bf0-105">指向承载为要显示的内容的 Web 部件进行筛选的页面的链接。</span><span class="sxs-lookup"><span data-stu-id="37bf0-105">Link to the page that host the Web part filtered for the content you want to display.</span></span> 
- <span data-ttu-id="37bf0-106">直接指向 Web 部件实例的链接</span><span class="sxs-lookup"><span data-stu-id="37bf0-106">Link directly to an instance of the Web part</span></span>

## <a name="link-to-a-page"></a><span data-ttu-id="37bf0-107">链接到页面</span><span class="sxs-lookup"><span data-stu-id="37bf0-107">Link to a page</span></span>

<span data-ttu-id="37bf0-108">如果您在自定义学习 Web 部件中创建了新的页面和学习体验, 则可以链接到该 Web 部件已配置为显示要显示的内容的页面。</span><span class="sxs-lookup"><span data-stu-id="37bf0-108">If you've created new pages and learning experiences with the Custom Learning Web part, you can link to the page with the Web part configured to show the content you want to display.</span></span> <span data-ttu-id="37bf0-109">在上一节中, 我们介绍了如何在页面上显示 Excel 播放列表。</span><span class="sxs-lookup"><span data-stu-id="37bf0-109">In the previous section, we covered how to display Excel playlists on a page.</span></span> <span data-ttu-id="37bf0-110">现在, 您可以编辑主页以链接到页面。</span><span class="sxs-lookup"><span data-stu-id="37bf0-110">You could now edit the Home page to link to the page.</span></span> 

1. <span data-ttu-id="37bf0-111">在主页中, 单击 "**编辑**"。</span><span class="sxs-lookup"><span data-stu-id="37bf0-111">From the Home page, click **Edit**.</span></span>
2. <span data-ttu-id="37bf0-112">单击其中一个主页磁贴中的 "**编辑详细信息**"。</span><span class="sxs-lookup"><span data-stu-id="37bf0-112">Click **Edit details** in one of the Home page tiles.</span></span> <span data-ttu-id="37bf0-113">在此示例中, 我们编辑**推荐的播放列表**磁贴。</span><span class="sxs-lookup"><span data-stu-id="37bf0-113">In this example, we edit the **Recommended playlists** tiles.</span></span>
3. <span data-ttu-id="37bf0-114">在 "**链接**" 下, 单击 "**更改**"。</span><span class="sxs-lookup"><span data-stu-id="37bf0-114">Under **Link**, click **Change**.</span></span>

![cg-linktopage](media/cg-linktopage.png)

4. <span data-ttu-id="37bf0-116">依次单击 "**网站**"、"**网站页面**" 和要链接到的页面, 然后单击 "**打开**"。</span><span class="sxs-lookup"><span data-stu-id="37bf0-116">Click **Site**, then **Site Pages**, click the page you want to link to, and then click **Open**.</span></span> <span data-ttu-id="37bf0-117">在此示例中, 我们将链接到上一节中介绍的**Create-your-own-experience**页。</span><span class="sxs-lookup"><span data-stu-id="37bf0-117">In this example, we link to the **Create-your-own-experience.aspx** page covered in the previous section.</span></span>
5. <span data-ttu-id="37bf0-118">关闭 "英雄属性" 窗格, 单击 "**发布**", 然后测试该链接。</span><span class="sxs-lookup"><span data-stu-id="37bf0-118">Close the Hero properties pane, click **Publish**, and then test the link.</span></span> 

## <a name="link-to-the-custom-learning-web-part"></a><span data-ttu-id="37bf0-119">链接到自定义学习 web 部件</span><span class="sxs-lookup"><span data-stu-id="37bf0-119">Link to the Custom Learning web part</span></span>
<span data-ttu-id="37bf0-120">自定义学习使您、管理员或最终用户能够链接到与包含 web 部件的页面无关的 web 部件实例。</span><span class="sxs-lookup"><span data-stu-id="37bf0-120">Custom Learning gives you, the administrator, or an end-user, the ability to link to an instance of the Web part independent of the page that contains the Web part.</span></span> <span data-ttu-id="37bf0-121">您可以将复制的链接或链接从其他页面共享。</span><span class="sxs-lookup"><span data-stu-id="37bf0-121">You can share the copied link or link to it from other pages.</span></span> <span data-ttu-id="37bf0-122">单击复制的链接时, 将在 CustomLLearningViewer 页中显示自定义学习 web 部件实例。</span><span class="sxs-lookup"><span data-stu-id="37bf0-122">The copied link, when clicked, shows the Custom Learning web part instance in the CustomLLearningViewer.aspx page.</span></span> <span data-ttu-id="37bf0-123">来看一个示例。</span><span class="sxs-lookup"><span data-stu-id="37bf0-123">Let's look at an example.</span></span> 

1. <span data-ttu-id="37bf0-124">在主页中, 单击 " **Office 365 培训**"。</span><span class="sxs-lookup"><span data-stu-id="37bf0-124">From the Home page, click **Office 365 training**.</span></span>
2. <span data-ttu-id="37bf0-125">单击 " **microsoft**团队", 然后单击 " **microsoft 团队简介**"。</span><span class="sxs-lookup"><span data-stu-id="37bf0-125">Click **Microsoft Teams**, and then click **Intro to Microsoft Teams**.</span></span>
3. <span data-ttu-id="37bf0-126">单击 "**复制**" 图标。</span><span class="sxs-lookup"><span data-stu-id="37bf0-126">Click the **Copy** icon.</span></span>

![cg-linktowebpart](media/cg-linktowebpart.png)

4. <span data-ttu-id="37bf0-128">从自定义学习菜单中单击 "主页"。</span><span class="sxs-lookup"><span data-stu-id="37bf0-128">Click Home from the Custom Learning menu.</span></span>
5. <span data-ttu-id="37bf0-129">将复制的 URL 粘贴到浏览器的地址栏中, 然后按 enter。</span><span class="sxs-lookup"><span data-stu-id="37bf0-129">Paste the copied URL in the address bar of the browser and press ENTER.</span></span> 

<span data-ttu-id="37bf0-130">如下图所示, 链接转到 CustomLearningViewer 页, 并根据复制的链接中的参数显示内容。</span><span class="sxs-lookup"><span data-stu-id="37bf0-130">As shown in the following illustration, the link goes to the CustomLearningViewer.aspx page and displays the content based on the parameters in the copied link.</span></span> 

![cg-linktowebpartviewer](media/cg-linktowebpartviewer.png)

