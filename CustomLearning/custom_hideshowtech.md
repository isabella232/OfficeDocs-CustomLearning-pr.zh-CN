---
author: pkrebs
ms.author: pkrebs
title: 隐藏和显示技术
ms.date: 02/15/2019
description: 如何隐藏和显示技术
ms.openlocfilehash: 38b814b85d4e060e5387b2173476c455cfcf7160
ms.sourcegitcommit: 775d6807291ab263eea5ec649d9aaf1933fb41ca
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/23/2019
ms.locfileid: "32055656"
---
# <a name="hide-and-show-technology"></a><span data-ttu-id="2300a-103">隐藏和显示技术</span><span class="sxs-lookup"><span data-stu-id="2300a-103">Hide and show Technology</span></span>

<span data-ttu-id="2300a-104">在某些情况下, 您可能希望隐藏组织中不支持的技术的内容。</span><span class="sxs-lookup"><span data-stu-id="2300a-104">In some cases, you’ll want to hide content for a technology that’s not supported in your organization.</span></span> <span data-ttu-id="2300a-105">隐藏技术功能旨在防止在整个 Web 部件中显示技术。</span><span class="sxs-lookup"><span data-stu-id="2300a-105">The Hide Technology feature is designed to prevent technology from appearing throughout the Web part.</span></span> <span data-ttu-id="2300a-106">它提供了一个更广泛的隐藏和显示内容的方法, 而不是通过子类别或播放列表隐藏内容。</span><span class="sxs-lookup"><span data-stu-id="2300a-106">It offers a broader way to hide and show content than hiding it by subcategory or playlist.</span></span> <span data-ttu-id="2300a-107">例如, 可以隐藏 yammer 子类别, 但 yammer 可能仍显示在某些方案播放列表中, 例如 "使用 Yammer 连接组织"。</span><span class="sxs-lookup"><span data-stu-id="2300a-107">For example, you can hide a Yammer subcategory, but Yammer may still show up in certain scenario playlists such as "Connect your organization with Yammer".</span></span> <span data-ttu-id="2300a-108">若要确保不会向最终用户公开特定技术, 可以通过技术隐藏它。</span><span class="sxs-lookup"><span data-stu-id="2300a-108">To ensure a specific technology is not exposed to end users, you can hide it by Technology.</span></span> 

## <a name="hide-a-technology"></a><span data-ttu-id="2300a-109">隐藏技术</span><span class="sxs-lookup"><span data-stu-id="2300a-109">Hide a Technology</span></span>

1. <span data-ttu-id="2300a-110">从自定义学习**主页**中, 单击 " **Office 365" 培训**磁贴。</span><span class="sxs-lookup"><span data-stu-id="2300a-110">From the Custom Learning **Home** page, click the **Office 365 training** tile.</span></span>
2. <span data-ttu-id="2300a-111">从自定义学习 Web 部件中, 选择 "**系统**" 菜单, 然后选择 "**管理播放列表**"。</span><span class="sxs-lookup"><span data-stu-id="2300a-111">From the Custom Learning Web part, select the **System** menu, then select **Administer Playlist**.</span></span> <span data-ttu-id="2300a-112">现在, 您应该打开两个选项卡。</span><span class="sxs-lookup"><span data-stu-id="2300a-112">You should now have two tabs open.</span></span> <span data-ttu-id="2300a-113">一个使用**自定义学习管理**页面, 另一个使用**Office 365 培训**页面。</span><span class="sxs-lookup"><span data-stu-id="2300a-113">One with the **Custom Learning Administration** page, and one with the **Office 365 training** page.</span></span> 
3. <span data-ttu-id="2300a-114">在 "**自定义学习管理**" 页上, 单击某一**技术**, 然后选择该技术要隐藏的 eyeball。</span><span class="sxs-lookup"><span data-stu-id="2300a-114">From the **Custom Learning Administration** page, click a **Technology**, and then select the eyeball for the Technology to hide it.</span></span> <span data-ttu-id="2300a-115">在此示例中, 单击**Yammer**技术, 然后将其隐藏。</span><span class="sxs-lookup"><span data-stu-id="2300a-115">For this example, click the **Yammer** technology, and then hide it.</span></span>  

![cg-hidetech](media/cg-hidetech.png)

### <a name="verify-the-playlist-is-hidden"></a><span data-ttu-id="2300a-117">验证是否隐藏了播放列表</span><span class="sxs-lookup"><span data-stu-id="2300a-117">Verify the playlist is hidden</span></span>
1. <span data-ttu-id="2300a-118">若要验证**Yammer**技术是否处于隐藏状态, 请在加载了**Office 365 培训**页的情况下选择 "浏览器" 选项卡, 然后刷新页面。</span><span class="sxs-lookup"><span data-stu-id="2300a-118">To verify **Yammer** technology is hidden, select the browser tab with the **Office 365 training** page loaded, and then refresh the page.</span></span> <span data-ttu-id="2300a-119">您现在应该会看到 "Yammer" 子类别处于隐藏状态。</span><span class="sxs-lookup"><span data-stu-id="2300a-119">You should now see the Yammer subcategory is hidden.</span></span> 
2. <span data-ttu-id="2300a-120">单击**推荐**的子类别。</span><span class="sxs-lookup"><span data-stu-id="2300a-120">Click the **Recommended** subcategory.</span></span> <span data-ttu-id="2300a-121">您会注意到, "使用 Yammer 连接组织" 播放列表处于隐藏状态。</span><span class="sxs-lookup"><span data-stu-id="2300a-121">You'll notice that the Connect your organization with Yammer playlist is hidden.</span></span> 

![cg-hidetechrefresh](media/cg-hidetechrefresh.png)

## <a name="unhide-a-technology"></a><span data-ttu-id="2300a-123">取消隐藏技术</span><span class="sxs-lookup"><span data-stu-id="2300a-123">Unhide a Technology</span></span>

- <span data-ttu-id="2300a-124">从 "**自定义学习管理**" 页面的 "**技术**" 下, 选择一种技术, 然后选择 "eyeball" 作为隐藏的技术以将其取消隐藏。</span><span class="sxs-lookup"><span data-stu-id="2300a-124">From the **Custom Learning Administration** page, under **Technology**, select a technology, then select the eyeball for the hidden technology to unhide it.</span></span> <span data-ttu-id="2300a-125">对于此示例, 请隐藏**Yammer**技术。</span><span class="sxs-lookup"><span data-stu-id="2300a-125">For this example, unhide the **Yammer** technology.</span></span> 