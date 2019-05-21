---
author: pkrebs
ms.author: pkrebs
title: Microsoft 365 学习通道安装选项
ms.date: 02/11/2019
description: 自定义学习设置的安装选项
ms.openlocfilehash: bef8e513d9126defc4b4f73acc6e07fc060044aa
ms.sourcegitcommit: 1a111a49a0413a56a880e29109ba01b5e5f33d09
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/20/2019
ms.locfileid: "34247687"
---
# <a name="learning-pathways-setup-options"></a><span data-ttu-id="ad0b7-103">学习路径安装选项</span><span class="sxs-lookup"><span data-stu-id="ad0b7-103">Learning pathways setup options</span></span>
<span data-ttu-id="ad0b7-104">通过学习路径, 可以灵活地以几种不同的方式设置解决方案。</span><span class="sxs-lookup"><span data-stu-id="ad0b7-104">Learning pathways provides the flexibility to set up the solution in a couple different ways.</span></span> <span data-ttu-id="ad0b7-105">以下各节概述了可用的选项。</span><span class="sxs-lookup"><span data-stu-id="ad0b7-105">The following sections outline the options available.</span></span>

## <a name="recommended---sharepoint-online-provisioning-service-setup"></a><span data-ttu-id="ad0b7-106">推荐-SharePoint Online 设置服务设置</span><span class="sxs-lookup"><span data-stu-id="ad0b7-106">Recommended - SharePoint Online Provisioning Service Setup</span></span> 
<span data-ttu-id="ad0b7-107">SharePoint Online 设置服务提供了设置自定义学习的最快、最方便和推荐方法。</span><span class="sxs-lookup"><span data-stu-id="ad0b7-107">The SharePoint Online Provisioning Service provides the fastest, easiest, and recommended method for setting up Custom Learning.</span></span> <span data-ttu-id="ad0b7-108">使用 SharePoint Online 设置服务, Office 365 租户管理员登录到服务, 进行几个选择, 然后单击 "**添加到租户**" 以设置自定义学习网站和自定义学习 Web 部件。</span><span class="sxs-lookup"><span data-stu-id="ad0b7-108">With the SharePoint Online Provisioning Service, an Office 365 tenant admin signs into the service, makes a few choices, and clicks **Add to Tenant** to provision the Custom Learning Site and the Custom Learning Web part.</span></span> <span data-ttu-id="ad0b7-109">设置完成后, 租户管理员会收到一封电子邮件, 指明网站已准备就绪。</span><span class="sxs-lookup"><span data-stu-id="ad0b7-109">When provisioning is done, the Tenant Admin receives an email that the site is ready to go.</span></span> 

- <span data-ttu-id="ad0b7-110">若要开始使用 SharePoint 设置服务, 请转到[PnP 预配服务](custom_provision.md)的 "预配"</span><span class="sxs-lookup"><span data-stu-id="ad0b7-110">To get started with the SharePoint Provisioning Service, go to [Provision with the PnP Provisioning Service](custom_provision.md)</span></span>   

## <a name="stand-alone-learning-pathways-web-part-setup"></a><span data-ttu-id="ad0b7-111">独立的学习路径 web 部件设置</span><span class="sxs-lookup"><span data-stu-id="ad0b7-111">Stand alone learning pathways web part setup</span></span>
<span data-ttu-id="ad0b7-112">对于已经建立了 SharePoint Online 新式通信培训门户的组织, 学习途径提供了将 Microsoft 365 学习路径 web 部件手动安装到现有 SharePoint Online 网站的选项。</span><span class="sxs-lookup"><span data-stu-id="ad0b7-112">For organizations that already have an established SharePoint Online modern communication training portal, learning pathways provides the option to manually install the Microsoft 365 learning pathways web part into an existing SharePoint Online site.</span></span> <span data-ttu-id="ad0b7-113">请注意, 该网站必须是新式 SharePoint Online 网站。</span><span class="sxs-lookup"><span data-stu-id="ad0b7-113">Note that the site must be a modern SharePoint Online site.</span></span> <span data-ttu-id="ad0b7-114">此方法需要租户管理权限和 Windows PowerShell 或 SharePoint Online 命令行管理程序的体验。</span><span class="sxs-lookup"><span data-stu-id="ad0b7-114">This method requires Tenant Admin permissions and experience with Windows PowerShell or the SharePoint Online Management Shell.</span></span> <span data-ttu-id="ad0b7-115">请注意, 此方法需要更多的技术专业知识, 然后 SharePoint Online 设置服务设置。</span><span class="sxs-lookup"><span data-stu-id="ad0b7-115">Note that this method requires more technical expertise then the SharePoint Online Provisioning Service setup.</span></span>

- <span data-ttu-id="ad0b7-116">有关手动 web 部件安装说明, 请参阅请参阅[手动安装 web 部件](custom_manualsetup.md)。</span><span class="sxs-lookup"><span data-stu-id="ad0b7-116">For Manual web part installation instructions, see see [Manually install the web part](custom_manualsetup.md).</span></span> 

## <a name="update-learning-pathways"></a><span data-ttu-id="ad0b7-117">更新学习路径</span><span class="sxs-lookup"><span data-stu-id="ad0b7-117">Update learning pathways</span></span>
<span data-ttu-id="ad0b7-118">已使用 SharePoint Online 设置服务来安装早期版本的 Microsoft 365 学习路径 (以前称为 Office 365 的自定义学习) 的组织可以将解决方案更新到最新版本。</span><span class="sxs-lookup"><span data-stu-id="ad0b7-118">Organizations that have used the SharePoint Online Provisioning Service to install earlier versions of Microsoft 365 learning pathways, previously called Custom Learning for Office 365,can update the solution to the latest version.</span></span> <span data-ttu-id="ad0b7-119">有关如何检查根据解决方案的最新版本部署的版本的说明, 以及有关如何更新解决方案的说明, 请参阅[自述文件](https://github.com/pnp/custom-learning-office-365/blob/master/README.md)的 "更新解决方案" 部分。</span><span class="sxs-lookup"><span data-stu-id="ad0b7-119">For instructions on how to check the version deployed against the most recent version of the solution, along with instructions on how to update the solution, see the "Updating the solution" section of the [ReadMe file](https://github.com/pnp/custom-learning-office-365/blob/master/README.md).</span></span>

### <a name="next-steps---provision-microsoft-365-learning-pathwayscustomprovisionmd"></a><span data-ttu-id="ad0b7-120">后续步骤-[预配 Microsoft 365 学习路径](custom_provision.md)</span><span class="sxs-lookup"><span data-stu-id="ad0b7-120">Next Steps - [Provision Microsoft 365 learning pathways](custom_provision.md)</span></span>
