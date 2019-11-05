---
author: pkrebs
ms.author: pkrebs
title: Microsoft 365 学习通道安装选项
ms.date: 02/11/2019
description: 自定义学习设置的安装选项
ms.openlocfilehash: 6906b5e70b186c106b3a9969b5bce1cbe87d7021
ms.sourcegitcommit: f4c2b6ef531d2d820c3d97871e187d0a2220d8f4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2019
ms.locfileid: "37956649"
---
# <a name="learning-pathways-setup-options"></a><span data-ttu-id="b06ef-103">学习路径安装选项</span><span class="sxs-lookup"><span data-stu-id="b06ef-103">Learning pathways setup options</span></span>
<span data-ttu-id="b06ef-104">通过学习路径，可以灵活地以几种不同的方式设置解决方案。</span><span class="sxs-lookup"><span data-stu-id="b06ef-104">Learning pathways provides the flexibility to set up the solution in a couple different ways.</span></span> <span data-ttu-id="b06ef-105">以下各节概述了可用的选项。</span><span class="sxs-lookup"><span data-stu-id="b06ef-105">The following sections outline the options available.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="b06ef-106">如果已为组织中的 Office 365 设置了自定义学习，并且想要更新解决方案，请按照[Microsoft 365 学习途径自述文件](https://github.com/pnp/custom-learning-office-365)中的 "更新解决方案" 说明操作。</span><span class="sxs-lookup"><span data-stu-id="b06ef-106">If you have already provisioned Custom Learning for Office 365 in your organization and want to update the solution, follow the “Updating the solution” instructions in the [Microsoft 365 learning pathways ReadMe](https://github.com/pnp/custom-learning-office-365).</span></span> <span data-ttu-id="b06ef-107">如果您是首次预配 Microsoft 365 学习路径，请参阅 Microsoft 365 学习通道文档中的[预配 microsoft 365 学习通道说明]( https://docs.microsoft.com/en-us/office365/customlearning/custom_provision)。</span><span class="sxs-lookup"><span data-stu-id="b06ef-107">If you are provisioning Microsoft 365 learning pathways for the first time, see [Provision Microsoft 365 learning pathways instructions]( https://docs.microsoft.com/en-us/office365/customlearning/custom_provision) in the Microsoft 365 learning pathways documentation.</span></span>  


## <a name="recommended---sharepoint-online-provisioning-service-setup"></a><span data-ttu-id="b06ef-108">推荐-SharePoint Online 设置服务设置</span><span class="sxs-lookup"><span data-stu-id="b06ef-108">Recommended - SharePoint Online Provisioning Service Setup</span></span> 
<span data-ttu-id="b06ef-109">SharePoint Online 设置服务提供了设置自定义学习的最快、最方便和推荐方法。</span><span class="sxs-lookup"><span data-stu-id="b06ef-109">The SharePoint Online Provisioning Service provides the fastest, easiest, and recommended method for setting up Custom Learning.</span></span> <span data-ttu-id="b06ef-110">使用 SharePoint Online 设置服务，Office 365 租户管理员登录到服务，进行几个选择，然后单击 "**添加到租户**" 以设置自定义学习网站和自定义学习 Web 部件。</span><span class="sxs-lookup"><span data-stu-id="b06ef-110">With the SharePoint Online Provisioning Service, an Office 365 tenant admin signs into the service, makes a few choices, and clicks **Add to Tenant** to provision the Custom Learning Site and the Custom Learning Web part.</span></span> <span data-ttu-id="b06ef-111">设置完成后，租户管理员会收到一封电子邮件，指明网站已准备就绪。</span><span class="sxs-lookup"><span data-stu-id="b06ef-111">When provisioning is done, the Tenant Admin receives an email that the site is ready to go.</span></span> 

- <span data-ttu-id="b06ef-112">若要开始使用 SharePoint 设置服务，请转到[PnP 预配服务](custom_provision.md)的 "预配"</span><span class="sxs-lookup"><span data-stu-id="b06ef-112">To get started with the SharePoint Provisioning Service, go to [Provision with the PnP Provisioning Service](custom_provision.md)</span></span>   

## <a name="stand-alone-learning-pathways-web-part-setup"></a><span data-ttu-id="b06ef-113">独立的学习路径 web 部件设置</span><span class="sxs-lookup"><span data-stu-id="b06ef-113">Stand alone learning pathways web part setup</span></span>
<span data-ttu-id="b06ef-114">对于已经建立了 SharePoint Online 新式通信培训门户的组织，学习途径提供了将 Microsoft 365 学习路径 web 部件手动安装到现有 SharePoint Online 网站的选项。</span><span class="sxs-lookup"><span data-stu-id="b06ef-114">For organizations that already have an established SharePoint Online modern communication training portal, learning pathways provides the option to manually install the Microsoft 365 learning pathways web part into an existing SharePoint Online site.</span></span> <span data-ttu-id="b06ef-115">请注意，该网站必须是新式 SharePoint Online 网站。</span><span class="sxs-lookup"><span data-stu-id="b06ef-115">Note that the site must be a modern SharePoint Online site.</span></span> <span data-ttu-id="b06ef-116">此方法需要租户管理权限和 Windows PowerShell 或 SharePoint Online 命令行管理程序的体验。</span><span class="sxs-lookup"><span data-stu-id="b06ef-116">This method requires Tenant Admin permissions and experience with Windows PowerShell or the SharePoint Online Management Shell.</span></span> <span data-ttu-id="b06ef-117">请注意，此方法需要更多的技术专业知识，然后 SharePoint Online 设置服务设置。</span><span class="sxs-lookup"><span data-stu-id="b06ef-117">Note that this method requires more technical expertise then the SharePoint Online Provisioning Service setup.</span></span>

- <span data-ttu-id="b06ef-118">有关手动 web 部件安装说明，请参阅请参阅[手动安装 web 部件](custom_manualsetup.md)。</span><span class="sxs-lookup"><span data-stu-id="b06ef-118">For Manual web part installation instructions, see see [Manually install the web part](custom_manualsetup.md).</span></span> 

## <a name="update-learning-pathways"></a><span data-ttu-id="b06ef-119">更新学习路径</span><span class="sxs-lookup"><span data-stu-id="b06ef-119">Update learning pathways</span></span>
<span data-ttu-id="b06ef-120">已使用 SharePoint Online 设置服务安装早期版本的 Microsoft 365 学习路径的组织可以将解决方案更新到最新版本。</span><span class="sxs-lookup"><span data-stu-id="b06ef-120">Organizations that have used the SharePoint Online Provisioning Service to install earlier versions of Microsoft 365 learning pathways can update the solution to the latest version.</span></span> <span data-ttu-id="b06ef-121">有关如何检查根据解决方案的最新版本部署的版本的说明，以及有关如何更新解决方案的说明，请参阅[自述文件](https://github.com/pnp/custom-learning-office-365/blob/master/README.md)的 "更新解决方案" 部分。</span><span class="sxs-lookup"><span data-stu-id="b06ef-121">For instructions on how to check the version deployed against the most recent version of the solution, along with instructions on how to update the solution, see the "Updating the solution" section of the [ReadMe file](https://github.com/pnp/custom-learning-office-365/blob/master/README.md).</span></span>

### <a name="next-steps---provision-microsoft-365-learning-pathwayscustom_provisionmd"></a><span data-ttu-id="b06ef-122">后续步骤-[预配 Microsoft 365 学习路径](custom_provision.md)</span><span class="sxs-lookup"><span data-stu-id="b06ef-122">Next Steps - [Provision Microsoft 365 learning pathways](custom_provision.md)</span></span>
