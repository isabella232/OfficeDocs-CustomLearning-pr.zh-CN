---
author: karuanag
ms.author: karuanag
title: 安装自定义学习解决方案 web 部件
ms.date: 02/10/2019
description: 自定义学习解决方案 web 部件的安装说明
ms.openlocfilehash: 53229e5b1b8175b06d888091963d1a9f2f0bd361
ms.sourcegitcommit: e10085e60ca3f38029fde229fb093e6bc4a34203
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/25/2019
ms.locfileid: "29989683"
---
# <a name="installing-the-custom-learning-solution-webpart"></a><span data-ttu-id="660c6-103">安装自定义学习解决方案 web 部件</span><span class="sxs-lookup"><span data-stu-id="660c6-103">Installing the Custom Learning Solution Webpart</span></span>

## <a name="prerequisites-for-a-tenant-wide-installation"></a><span data-ttu-id="660c6-104">租户范围安装的先决条件</span><span class="sxs-lookup"><span data-stu-id="660c6-104">Prerequisites for a tenant-wide installation</span></span>

- <span data-ttu-id="660c6-p101">若要为你的整个租户安装自定义的学习 web 部件, 你需要具有 Office 365 管理权限。 如果您没有这些权限, 则可以与 Office 365 管理员合作, 也可以为单个网站集安装 web 部件。</span><span class="sxs-lookup"><span data-stu-id="660c6-p101">To install the Custom Learning webpart for your entire tenant you will need to have Office 365 Administrative permissions.  If you do not have these permissions you can either work with your Office 365 Administrator or install the webpart for an individual site collection.</span></span>
- <span data-ttu-id="660c6-107">您或您的 Office 365 管理员必须已安装并配置了租户范围的[应用程序目录](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/set-up-your-developer-tenant)或[网站集应用程序目录](https://docs.microsoft.com/en-us/sharepoint/dev/general-development/site-collection-app-catalog), 才能接收 web 部件。]</span><span class="sxs-lookup"><span data-stu-id="660c6-107">You or your Office 365 Administrator must have setup and configured a tenant-wide [App Catalog](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/set-up-your-developer-tenant) or a [Site Collection App Catalog](https://docs.microsoft.com/en-us/sharepoint/dev/general-development/site-collection-app-catalog)to receive the webpart.]</span></span>
- <span data-ttu-id="660c6-p102">我们仅支持 SharePoint Online。web 部件不支持在本地的任何 SharePoint 版本上安装。</span><span class="sxs-lookup"><span data-stu-id="660c6-p102">We support SharePoint Online only. The web part is not support for installation on any version of SharePoint on premises.</span></span>

## <a name="add-the-custom-learning-webpart-to-your-tenant"></a><span data-ttu-id="660c6-110">将自定义学习 web 部件添加到租户</span><span class="sxs-lookup"><span data-stu-id="660c6-110">Add the Custom Learning webpart to your tenant</span></span> 

1. <span data-ttu-id="660c6-p103">下载自定义学习 web 部件并将其保存到本地驱动器。 此文件名为 "ms-自定义 .sppkg"。 不要更改文件的名称或后缀。</span><span class="sxs-lookup"><span data-stu-id="660c6-p103">Download the Custom Learning webpart and save it to your local drive.  This file is named "ms-custom-learning.sppkg".  Do not change the name or suffix of the file.</span></span> 
2. <span data-ttu-id="660c6-114">导航到适用于租户的[Office 365 管理门户](https://admin.microsoft.com/AdminPortal/Home#/homepage)</span><span class="sxs-lookup"><span data-stu-id="660c6-114">Navigate to the [Office 365 Admin portal](https://admin.microsoft.com/AdminPortal/Home#/homepage) for your tenant</span></span>
3. <span data-ttu-id="660c6-p104">从左侧导航中选择 "管理中心"、"SharePoint"。这将在新选项卡中打开。, 在 SharePoint 管理中心中选择 "应用程序"、"应用程序目录" 和 "SharePoint 相关应用程序"</span><span class="sxs-lookup"><span data-stu-id="660c6-p104">From the left navigation select Admin Centers, SharePoint. This will open in a new tab. , In the SharePoint Admin Center select Apps, App Catalog, Apps for SharePoint</span></span> 
4. <span data-ttu-id="660c6-117">选择 "上载 web 部件", 然后选择您下载的 "ms-自定义 .sppkg" 文件</span><span class="sxs-lookup"><span data-stu-id="660c6-117">Select upload the webpart and choose the "ms-custom-learning.sppkg" file you downloaded</span></span>
5. <span data-ttu-id="660c6-118">对于此租户范围的安装, 请选中 "使此解决方案可供组织中的所有公司使用" 旁边的复选框。</span><span class="sxs-lookup"><span data-stu-id="660c6-118">For this tenant-wide installation check the box next to "Make this solution available to all sits in the organization."</span></span>  
 
> [!NOTE]
> <span data-ttu-id="660c6-p105">安装 webpart 后, 即可在 SharePoint Online 的 web 部件库中找到它。 **在库中, web 部件名为 "Microsoft 学习"**</span><span class="sxs-lookup"><span data-stu-id="660c6-p105">Once the webpart is installed you will find it in your webpart gallery in SharePoint Online.  **In the gallery the webpart is named "Microsoft Learning"**</span></span>

![部署解决方案](media/trustapp_sm.png)


## <a name="add-the-microsoft-learning-webpart-to-a-sharepoint-online-page"></a><span data-ttu-id="660c6-122">将 Microsoft 学习 web 部件添加到 SharePoint Online 页面</span><span class="sxs-lookup"><span data-stu-id="660c6-122">Add the Microsoft Learning webpart to a SharePoint Online Page</span></span>

<span data-ttu-id="660c6-p106">在租户中安装自定义学习后, 可以将 Web 部件添加到 SharePoint 页面。当你执行 Office 365 和 Windows 10 培训时, 你的网站可供你使用。</span><span class="sxs-lookup"><span data-stu-id="660c6-p106">After Custom Learning is installed in your tenant you can add the Web part to a SharePoint page. When you do Office 365 and Windows 10 training is available to your site.</span></span>

1. <span data-ttu-id="660c6-125">在全宽列布局中添加自定义学习 web 部件:</span><span class="sxs-lookup"><span data-stu-id="660c6-125">Add the Custom Learning webpart in a full width column layout:</span></span>

![SharePoint 页面布局](media/clo365fullcolumnwidth.png)

2. <span data-ttu-id="660c6-p107">在 SharePoint 页面中, 选择 "添加内容", 然后选择 "全宽列"。 您将看到以下提示:</span><span class="sxs-lookup"><span data-stu-id="660c6-p107">In the SharePoint page, select Add section and then select full width column.  You'll see the following prompt:</span></span>

![AddWebpart](media/clo365addfullwidthwebpart.png)

3. <span data-ttu-id="660c6-p108">选择 "Microsoft 学习"。 您现在应该会看到以下内容:</span><span class="sxs-lookup"><span data-stu-id="660c6-p108">Select Microsoft Learning.  You should now see the following:</span></span> 

![自定义学习 web 部件](media/clo365addwebpart.png)

 <span data-ttu-id="660c6-133">您现在可以单击磁贴来浏览解决方案中包含的默认内容。</span><span class="sxs-lookup"><span data-stu-id="660c6-133">You can now click on the tiles to explore the default content included in the solution.</span></span>  

### <a name="next-steps"></a><span data-ttu-id="660c6-134">后续步骤</span><span class="sxs-lookup"><span data-stu-id="660c6-134">Next Steps</span></span>
- <span data-ttu-id="660c6-135">浏览 web 部件中包含的[默认内容](webpartcontent.md)。</span><span class="sxs-lookup"><span data-stu-id="660c6-135">Explore the [default content](webpartcontent.md) included in the webpart.</span></span>
- <span data-ttu-id="660c6-136">为你的组织[自定义](customization.md)培训体验。</span><span class="sxs-lookup"><span data-stu-id="660c6-136">[Customize](customization.md) the training experience for your organization.</span></span>
- <span data-ttu-id="660c6-137">[促进](driveadoption.md)培训解决方案的采用。</span><span class="sxs-lookup"><span data-stu-id="660c6-137">[Drive adoption](driveadoption.md) of your training solution.</span></span>

