---
author: pkrebs
ms.author: pkrebs
title: 隐藏和显示技术
ms.date: 05/20/2019
description: 如何隐藏和显示技术
ms.openlocfilehash: ee943dad5ca3f2a1bef5636e0f820346b0ac3840
ms.sourcegitcommit: f5a7079d56598c14aef2f4b886c025a59ba89276
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/21/2019
ms.locfileid: "34327263"
---
# <a name="hide-and-show-technology"></a><span data-ttu-id="d6450-103">隐藏和显示技术</span><span class="sxs-lookup"><span data-stu-id="d6450-103">Hide and show Technology</span></span>

<span data-ttu-id="d6450-104">在某些情况下，您可能希望隐藏组织中不支持的技术的内容。</span><span class="sxs-lookup"><span data-stu-id="d6450-104">In some cases, you’ll want to hide content for a technology that’s not supported in your organization.</span></span> <span data-ttu-id="d6450-105">隐藏技术功能旨在防止在整个 Web 部件中显示技术。</span><span class="sxs-lookup"><span data-stu-id="d6450-105">The Hide Technology feature is designed to prevent technology from appearing throughout the Web part.</span></span> <span data-ttu-id="d6450-106">它提供了一个更广泛的隐藏和显示内容的方法，而不是通过子类别或播放列表隐藏内容。</span><span class="sxs-lookup"><span data-stu-id="d6450-106">It offers a broader way to hide and show content than hiding it by subcategory or playlist.</span></span> <span data-ttu-id="d6450-107">例如，可以隐藏 Yammer 子类别，但 Yammer 可能仍显示在某些方案播放列表中，例如 "使用 Yammer 连接组织"。</span><span class="sxs-lookup"><span data-stu-id="d6450-107">For example, you can hide a Yammer subcategory, but Yammer may still show up in certain scenario playlists such as "Connect your organization with Yammer".</span></span> <span data-ttu-id="d6450-108">若要确保不会向最终用户公开特定技术，可以通过技术隐藏它。</span><span class="sxs-lookup"><span data-stu-id="d6450-108">To ensure a specific technology is not exposed to end users, you can hide it by Technology.</span></span> 

## <a name="hide-a-technology"></a><span data-ttu-id="d6450-109">隐藏技术</span><span class="sxs-lookup"><span data-stu-id="d6450-109">Hide a Technology</span></span>

1. <span data-ttu-id="d6450-110">在 Microsoft 365 学习路径**主页**中，单击推荐的**播放列表**磁贴。</span><span class="sxs-lookup"><span data-stu-id="d6450-110">From the Microsoft 365 learning pathways **Home** page, click the **Recommended playlists** tile.</span></span>
2. <span data-ttu-id="d6450-111">从自定义学习 Web 部件中，选择 "**系统**" 菜单，然后选择 "**管理播放列表**"。</span><span class="sxs-lookup"><span data-stu-id="d6450-111">From the Custom Learning Web part, select the **System** menu, then select **Administer Playlist**.</span></span> <span data-ttu-id="d6450-112">现在，您应该打开两个选项卡。</span><span class="sxs-lookup"><span data-stu-id="d6450-112">You should now have two tabs open.</span></span> <span data-ttu-id="d6450-113">一个包含**建议的播放列表**页面，另一个使用**自定义学习管理**页面。</span><span class="sxs-lookup"><span data-stu-id="d6450-113">One with the **Recommended playlists** page, and one with the **Custom Learning Administration** page.</span></span> 
3. <span data-ttu-id="d6450-114">在 "**自定义学习管理**" 页上，单击某一**技术**，然后选择该技术要隐藏的 eyeball。</span><span class="sxs-lookup"><span data-stu-id="d6450-114">From the **Custom Learning Administration** page, click a **Technology**, and then select the eyeball for the technology to hide it.</span></span> <span data-ttu-id="d6450-115">在此示例中，单击**Yammer**技术，然后将其隐藏。</span><span class="sxs-lookup"><span data-stu-id="d6450-115">For this example, click the **Yammer** technology, and then hide it.</span></span>  

![cg-hidetech](media/cg-hidetech.png)

### <a name="verify-the-playlist-is-hidden"></a><span data-ttu-id="d6450-117">验证是否隐藏了播放列表</span><span class="sxs-lookup"><span data-stu-id="d6450-117">Verify the playlist is hidden</span></span>
- <span data-ttu-id="d6450-118">若要验证**Yammer**技术是否处于隐藏状态，请选择 "浏览器" 选项卡，并加载**建议的播放列表**页，然后刷新页面。</span><span class="sxs-lookup"><span data-stu-id="d6450-118">To verify **Yammer** technology is hidden, select the browser tab with the **Recommended playlists** page loaded, and then refresh the page.</span></span> <span data-ttu-id="d6450-119">您会注意到，"使用 Yammer 连接组织" 播放列表处于隐藏状态。</span><span class="sxs-lookup"><span data-stu-id="d6450-119">You'll notice that the Connect your organization with Yammer playlist is hidden.</span></span> 

![cg-hidetechrefresh](media/cg-hidetechrefresh.png)

## <a name="unhide-a-technology"></a><span data-ttu-id="d6450-121">取消隐藏技术</span><span class="sxs-lookup"><span data-stu-id="d6450-121">Unhide a Technology</span></span>

- <span data-ttu-id="d6450-122">从 "**自定义学习管理**" 页面的 "**技术**" 下，选择一种技术，然后选择 "eyeball" 作为隐藏的技术以将其取消隐藏。</span><span class="sxs-lookup"><span data-stu-id="d6450-122">From the **Custom Learning Administration** page, under **Technology**, select a technology, then select the eyeball for the hidden technology to unhide it.</span></span> <span data-ttu-id="d6450-123">对于此示例，请隐藏**Yammer**技术。</span><span class="sxs-lookup"><span data-stu-id="d6450-123">For this example, unhide the **Yammer** technology.</span></span> 