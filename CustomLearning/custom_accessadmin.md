---
author: pkrebs
ms.author: pkrebs
title: 学习路径管理
ms.date: 02/15/2019
description: 如何从 Web 部件或菜单访问自定义学习管理页
ms.openlocfilehash: 86526f4c4b3d46360ab2c63a503bfd80e0848c13
ms.sourcegitcommit: 3b8896c81ad2adbcfdbda658482847af5fccb264
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/30/2019
ms.locfileid: "37886927"
---
# <a name="access-the-learning-pathways-administration-page"></a><span data-ttu-id="04211-103">访问 "学习路径管理" 页</span><span class="sxs-lookup"><span data-stu-id="04211-103">Access the Learning Pathways Administration page</span></span>

<span data-ttu-id="04211-104">学习路径管理是从 CustomLearningAdmin 页面进行管理。</span><span class="sxs-lookup"><span data-stu-id="04211-104">Learning pathways administration is managed from the CustomLearningAdmin.aspx page.</span></span> <span data-ttu-id="04211-105">此管理页仅适用于 SharePoint 管理员。</span><span class="sxs-lookup"><span data-stu-id="04211-105">This administration page is only available to SharePoint Administrators.</span></span> <span data-ttu-id="04211-106">拥有访问此网站的成员权限的用户将不会在 Web 部件上看到**管理**齿轮图标。</span><span class="sxs-lookup"><span data-stu-id="04211-106">Users with member privileges visiting the site will not see the **Administration** gear icon on the Web part.</span></span> <span data-ttu-id="04211-107">此外，只有管理员能够从 SharePoint**主页**菜单下的 "**学习路径管理**" 菜单项打开 "管理" 页面。</span><span class="sxs-lookup"><span data-stu-id="04211-107">In addition, only Administrators will have the ability to open the administration page from the **Learning pathways administration** menu item under the SharePoint **Home** menu.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="04211-108">在自定义学习管理页上所做的更改（如隐藏产品子类别或播放列表）将在 Web 部件的所有实例中反映出来。</span><span class="sxs-lookup"><span data-stu-id="04211-108">Changes made on the Custom Learning Administration page, such as hiding a product subcategory or playlist, will be reflected in all instances of the Web part.</span></span> <span data-ttu-id="04211-109">此外，建议一次仅有一个管理员从管理页面进行更改，因为如果有多个用户同时使用该页面，自定义学习不会提供冲突检测。</span><span class="sxs-lookup"><span data-stu-id="04211-109">In addition, it’s recommended that only one administrator at time make changes from the administration page, since Custom Learning does not provide collision detection if multiple people are using the page at the same time.</span></span>  

## <a name="access-from-the-learning-pathways-web-part---preferred-method"></a><span data-ttu-id="04211-110">从 "学习路径 web 部件-首选" 方法访问</span><span class="sxs-lookup"><span data-stu-id="04211-110">Access from the Learning pathways web part - preferred method</span></span>
<span data-ttu-id="04211-111">从 web 部件打开管理页是首选方法，因为它在新的浏览器选项卡中打开页面。使用此方法，可以在选项卡式页面之间来回翻转以检查或修改您的工作。</span><span class="sxs-lookup"><span data-stu-id="04211-111">Opening the Administration page from the web part is the preferred method since it opens the page in a new browser tab. With this method, it's easy to flip back and forth between the tabbed pages to check or modify your work.</span></span>  

1. <span data-ttu-id="04211-112">在 Microsoft 365 学习路径**主页**中，单击**Office 365 培训**磁贴。</span><span class="sxs-lookup"><span data-stu-id="04211-112">From the Microsoft 365 learning pathways **Home** page, click the **Office 365 training** tile.</span></span>
2. <span data-ttu-id="04211-113">单击 Web 部件中的 "**管理**" 图标，如下面的示例所示</span><span class="sxs-lookup"><span data-stu-id="04211-113">Click the **Administration** icon in the Web part as shown in the following example</span></span>  

![cg-adminaccbtn](media/cg-adminaccbtn.png)

## <a name="access-from-the-home-menu-item"></a><span data-ttu-id="04211-115">从 "主页" 菜单项访问</span><span class="sxs-lookup"><span data-stu-id="04211-115">Access from the Home menu item</span></span>
<span data-ttu-id="04211-116">管理员可以从 SharePoint**主页**菜单项访问 "管理" 页面，而不是导航到包含 Web 部件的页面。</span><span class="sxs-lookup"><span data-stu-id="04211-116">Rather than navigate to a page with a Web part, administrators can access the Adminstration page from the SharePoint **Home** menu item.</span></span> 

- <span data-ttu-id="04211-117">在 Microsoft 365 学习路径主页中，单击 "**主页**" 菜单，然后单击 " **Microsoft 学习管理**"。</span><span class="sxs-lookup"><span data-stu-id="04211-117">From the Microsoft 365 Learning Pathways Home page, click the **Home** menu, then click **Microsoft learning administration**.</span></span>

![cg-adminaccmenu](media/cg-adminaccmenu.png)