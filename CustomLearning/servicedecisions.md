---
author: karuanag
ms.author: karuanag
title: 先决条件和决策
ms.date: 02/10/2019
description: 自定义学习安装和设置的决策和预备信息
ms.openlocfilehash: b7864d13e6ccd9c3b41e445ea491aed3b3471aff
ms.sourcegitcommit: 775d6807291ab263eea5ec649d9aaf1933fb41ca
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/23/2019
ms.locfileid: "32055262"
---
## <a name="service-decisions"></a><span data-ttu-id="1e1a1-103">服务决策</span><span class="sxs-lookup"><span data-stu-id="1e1a1-103">Service Decisions</span></span>

<span data-ttu-id="1e1a1-104">在确保已满足自定义学习的先决条件后, 您需要对 implemenation 的自定义学习做出以下决策:</span><span class="sxs-lookup"><span data-stu-id="1e1a1-104">After you've ensured that the prerequisites for Custom Learning have been met, you'll need to make the following decisions about your implemenation of Custom Learning:</span></span>

1. <span data-ttu-id="1e1a1-105">**您的公司中是否已有一个带有新式接口的培训门户？**</span><span class="sxs-lookup"><span data-stu-id="1e1a1-105">**Do you already have a training portal in your company with a modern interface?**</span></span>

- <span data-ttu-id="1e1a1-106">**是**如果你对这些问题的回答是肯定的, 则在现有网站体验中[安装 web 部件](installwebpart.md)是我们建议的操作过程。</span><span class="sxs-lookup"><span data-stu-id="1e1a1-106">**YES** If your answer to these questions are yes, then [installing the webpart](installwebpart.md) within that existing site experience is our recommended course of action.</span></span>
- <span data-ttu-id="1e1a1-107">**否**如果你回答 "否", 则建议[安装完整的自定义学习网站](installsitepackage.md)程序包。</span><span class="sxs-lookup"><span data-stu-id="1e1a1-107">**NO** If you answer no we suggest [installing the full Custom Learning site](installsitepackage.md) package.</span></span>  <span data-ttu-id="1e1a1-108">这将为您准备好一个新式的 SharePoint Online 通信网站, 您可以扩展该网站, 以容纳对最终用户重要的其他信息。</span><span class="sxs-lookup"><span data-stu-id="1e1a1-108">This will prepare you with a modern SharePoint Online communication site that your can expand to house other information that is important to your end users.</span></span>  <span data-ttu-id="1e1a1-109">自定义网站不会影响 web 部件获取内容更新的能力。</span><span class="sxs-lookup"><span data-stu-id="1e1a1-109">Customizing the site will not impact the webpart's ability to get content updates.</span></span> 

2. <span data-ttu-id="1e1a1-110">**您是 Office 365 管理员吗？**</span><span class="sxs-lookup"><span data-stu-id="1e1a1-110">**Are you an Office 365 Administrator?**</span></span>

- <span data-ttu-id="1e1a1-111">**是**: 您对这两种安装都拥有适当的权限。</span><span class="sxs-lookup"><span data-stu-id="1e1a1-111">**YES**:  You have the appropriate rights for either installation.</span></span>
- <span data-ttu-id="1e1a1-112">**NO**: 联系 Office 365 管理员以获取帮助或在你拥有的网站集中安装 web 部件</span><span class="sxs-lookup"><span data-stu-id="1e1a1-112">**NO**: Contact your Office 365 Administrator for assistance or install the webpart in a site collection you own</span></span>

3. <span data-ttu-id="1e1a1-113">**您是否在组织中有正式的培训部门？**</span><span class="sxs-lookup"><span data-stu-id="1e1a1-113">**Do you have a formal training department in your organization?**</span></span>

- <span data-ttu-id="1e1a1-114">**是**: 请确保将其接洽, 并让他们了解如何使用这些解决方案来提供其他自定义的培训内容。</span><span class="sxs-lookup"><span data-stu-id="1e1a1-114">**YES**:  Make sure to engage them and let them know how they can use these solutions to deliver additional, customized training content.</span></span>
- <span data-ttu-id="1e1a1-115">**否**: 使用我们的[自助服务采用工具包](driveadoption.md), 让最终用户知道网站可提供帮助。</span><span class="sxs-lookup"><span data-stu-id="1e1a1-115">**NO**:  Use our [self service adoption kit](driveadoption.md) to make your end-users aware the site is available to help them.</span></span>

4. <span data-ttu-id="1e1a1-116">**您的组织中是否有用户社区？ 这是一组正式或非正式用户, 他们希望了解有关技术的详细信息, 有时称为 "高级用户", 或者只是那些想要了解详细信息的人。**</span><span class="sxs-lookup"><span data-stu-id="1e1a1-116">**Do you have a user community in your organization?  This would be either a formal or informal group of users who like to know more about technology, sometimes called power users or just those interested to learn more.**</span></span>

- <span data-ttu-id="1e1a1-117">**是**: 您可以使用自定义学习网站体验提供指向任何新的或现有的用户社区论坛的链接。</span><span class="sxs-lookup"><span data-stu-id="1e1a1-117">**YES**:  You can use the Custom Learning site experience to provide links to any new or existing user community forums.</span></span>
- <span data-ttu-id="1e1a1-118">**否**: 考虑启动内部用户组, 以便用户可以共享其成功并彼此了解。</span><span class="sxs-lookup"><span data-stu-id="1e1a1-118">**NO**:  Consider starting an internal user group so people can share their success and learn from each other.</span></span>  <span data-ttu-id="1e1a1-119">如果你没有时间培养内部用户组, 并且你的员工可以加入[Microosft office 365 冠军社区](https://aka.ms/O365Champions)以进行月度培训, 在线社区中的成员资格和早期访问 Office 365 的工具和资源。</span><span class="sxs-lookup"><span data-stu-id="1e1a1-119">If you don't have time to nurture an internal user group you and your employees can join the [Microosft Office 365 Champion community](https://aka.ms/O365Champions) for monthly training, membership in the online community and early access to tools and resources for Office 365.</span></span>

5.  <span data-ttu-id="1e1a1-120">**您是否负责网站维护或支持问题？**</span><span class="sxs-lookup"><span data-stu-id="1e1a1-120">**Will you be accountable for site maintenance or support questions?**</span></span>

- <span data-ttu-id="1e1a1-121">**是**: 建议使用 Office 365 的功能, 以简化自定义的学习网站支持。</span><span class="sxs-lookup"><span data-stu-id="1e1a1-121">**YES**: We suggest using the capabilities of Office 365 to make Custom Learning site support easier.</span></span>  <span data-ttu-id="1e1a1-122">根据您的服务订阅和组织大小, 有些想法为:</span><span class="sxs-lookup"><span data-stu-id="1e1a1-122">Some ideas, depending on your service subscription and organization size are:</span></span>
    1. <span data-ttu-id="1e1a1-123">大型组织可以预配一个公共 Yammer 社区, 以获取有关网站的反馈</span><span class="sxs-lookup"><span data-stu-id="1e1a1-123">Large organizations can provision a public Yammer community to get feedback on the site</span></span>
    2. <span data-ttu-id="1e1a1-124">最高为2500的人员可以加入 Microsoft 团队, 以提出问题并共享对话</span><span class="sxs-lookup"><span data-stu-id="1e1a1-124">Up to 2500 people can join a Microsoft Team to ask questions and share conversation</span></span>
    3. <span data-ttu-id="1e1a1-125">正式的支持票证处理流程可以通过表单、流和 SharePoint Online 列表进行 suppored, 也可以通过您可能已在公司中支持 IT 支持的其他第三方工具来完成。</span><span class="sxs-lookup"><span data-stu-id="1e1a1-125">A formal support ticketing process can be suppored with Forms, Flow and SharePoint Online lists or through other 3rd party tools which you may already have for IT support in your company.</span></span> 
- <span data-ttu-id="1e1a1-126">**否**: 与提供 SharePoint Online 支持的 IT 员工讨论网站/web 部件的安装。</span><span class="sxs-lookup"><span data-stu-id="1e1a1-126">**NO**:  Discuss the installation of the site/webpart with your IT staff who provide SharePoint Online support.</span></span>  

### <a name="next-steps---site-provisioninginstallsitepackagemd-or-webpartinstallwebpartmd-installation-steps"></a><span data-ttu-id="1e1a1-127">后续步骤-[网站设置](installsitepackage.md)或[web 部件](installwebpart.md)安装步骤</span><span class="sxs-lookup"><span data-stu-id="1e1a1-127">Next Steps - [Site Provisioning](installsitepackage.md) or [webpart](installwebpart.md) installation steps</span></span>