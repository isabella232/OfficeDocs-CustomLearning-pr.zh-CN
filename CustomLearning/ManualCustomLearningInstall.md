---
author: pkrebs
ms.author: pkrebs
title: 手动安装学习路径
ms.date: 02/18/2019
description: 手动安装学习路径
ms.service: sharepoint online
ms.openlocfilehash: 992fe28f1ca2bdd09c5d29a4a5342b06ff093105
ms.sourcegitcommit: 907c657e7cc5a4a44d2b9f38cc35fea9ac5c5943
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/24/2021
ms.locfileid: "51162839"
---
# <a name="manually-installing-and-configuring-custom-learning-for-office-365"></a><span data-ttu-id="130a4-103">手动安装和配置 Office 365 的自定义学习</span><span class="sxs-lookup"><span data-stu-id="130a4-103">Manually installing and configuring Custom Learning for Office 365</span></span>

<span data-ttu-id="130a4-104">Microsoft 自定义学习Web 部件 [使用 SharePoint 框架](/sharepoint/dev/spfx/sharepoint-framework-overview) 版本 1.7.1 生成。</span><span class="sxs-lookup"><span data-stu-id="130a4-104">The Microsoft Custom Learning Web Part is build using the [SharePoint Framework](/sharepoint/dev/spfx/sharepoint-framework-overview) version 1.7.1.</span></span>

<span data-ttu-id="130a4-105">若要手动安装和配置 Web 部件和网站集，需要完成以下步骤：</span><span class="sxs-lookup"><span data-stu-id="130a4-105">To manually install and configure the web part and site collection you will need to complete the following steps:</span></span>

1. <span data-ttu-id="130a4-106">验证是否满足所有先决条件。</span><span class="sxs-lookup"><span data-stu-id="130a4-106">Validate that you have met all the prerequisites.</span></span>
1. <span data-ttu-id="130a4-107">在 Office 365 租户应用程序目录中安装 customlearning.sppkg 文件。</span><span class="sxs-lookup"><span data-stu-id="130a4-107">Install the customlearning.sppkg file in your Office 365 Tenant App Catalog.</span></span>
1. <span data-ttu-id="130a4-108">设置/标识新式通信网站，以用作 Office 365 自定义学习主网站。</span><span class="sxs-lookup"><span data-stu-id="130a4-108">Provision/Identify a modern communication site to act as your Custom Learning for Office 365 home site.</span></span>
1. <span data-ttu-id="130a4-109">执行 PowerShell 脚本，该脚本使用自定义学习所依赖的适当项目配置租户。</span><span class="sxs-lookup"><span data-stu-id="130a4-109">Execute a PowerShell script that will configure your tenant with the appropriate artifacts that Custom Learning depends on.</span></span>
1. <span data-ttu-id="130a4-110">导航到 CustomLearningAdmin.aspx 网站页面，以加载管理员 Web 部件以初始化自定义内容配置。</span><span class="sxs-lookup"><span data-stu-id="130a4-110">Navigate to the CustomLearningAdmin.aspx site page to load the admin web part to initialize the custom content configuration.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="130a4-111">先决条件</span><span class="sxs-lookup"><span data-stu-id="130a4-111">Prerequisites</span></span>

<span data-ttu-id="130a4-112">你必须已设置和配置租户范围的应用程序目录。</span><span class="sxs-lookup"><span data-stu-id="130a4-112">You must have set up and configured the tenant-wide App Catalog.</span></span> <span data-ttu-id="130a4-113">请参阅 [设置 Office 365 租户并按照](/sharepoint/dev/spfx/set-up-your-developer-tenant#create-app-catalog-site) 创建应用程序目录网站部分操作。</span><span class="sxs-lookup"><span data-stu-id="130a4-113">Please see [Set up your Office 365 tenant](/sharepoint/dev/spfx/set-up-your-developer-tenant#create-app-catalog-site) and follow the Create app catalog site section.</span></span> <span data-ttu-id="130a4-114">如果租户范围的应用程序目录已预配，则需要访问具有将程序包上载到该帐户权限的帐户才能完成此设置过程。</span><span class="sxs-lookup"><span data-stu-id="130a4-114">If your tenant-wide App Catalog has already been provisioned you will need access to an account that has rights to upload a package to it to complete this setup process.</span></span> <span data-ttu-id="130a4-115">通常，这是具有 SharePoint 管理员角色的帐户。</span><span class="sxs-lookup"><span data-stu-id="130a4-115">Generally this is an account with the SharePoint administrator role.</span></span> <span data-ttu-id="130a4-116">如果具有该角色的帐户不起作用，请转到 SharePoint 管理中心并查找应用程序目录网站集的网站集管理员，并作为网站集管理员之一登录，或者向网站集管理员添加失败的 SharePoint 管理员帐户。</span><span class="sxs-lookup"><span data-stu-id="130a4-116">If an account with that role does not work, go to the SharePoint admin center and find the Site Collection Administrators for the app catalog site collection and either log in as one of the Site Collection Administrators, or add the SharePoint administrator account that failed to the Site Collection Administrators.</span></span> <span data-ttu-id="130a4-117">你还需要访问作为 SharePoint 租户管理员的帐户。</span><span class="sxs-lookup"><span data-stu-id="130a4-117">You will also need access to an account that is a SharePoint Tenant Admin.</span></span>

## <a name="upload-the-web-part-to-the-tenant-app-catalog"></a><span data-ttu-id="130a4-118">将 Web 部件上载到租户应用程序目录</span><span class="sxs-lookup"><span data-stu-id="130a4-118">Upload the web part to the Tenant App Catalog</span></span>

<span data-ttu-id="130a4-119">若要设置 Office 365 的自定义学习，您需要将 customlearning.sppkg 文件上载到租户范围的应用程序目录并部署它。</span><span class="sxs-lookup"><span data-stu-id="130a4-119">To set up Custom Learning for Office 365, you upload the customlearning.sppkg file to the tenant-wide App Catalog and deploy it.</span></span> <span data-ttu-id="130a4-120">有关如何 [将应用程序添加到](/sharepoint/use-app-catalog) 应用程序目录的详细说明，请参阅使用应用程序目录为 SharePoint Online 环境提供自定义业务应用程序。</span><span class="sxs-lookup"><span data-stu-id="130a4-120">Please see [Use the App Catalog to make custom business apps available for your SharePoint Online environment](/sharepoint/use-app-catalog) for detailed instructions on how to add an app to the app catalog.</span></span>

## <a name="provisionidentify-modern-communication-site"></a><span data-ttu-id="130a4-121">预配/识别新式通信网站</span><span class="sxs-lookup"><span data-stu-id="130a4-121">Provision/Identify Modern Communication Site</span></span>

<span data-ttu-id="130a4-122">确定现有 SharePoint 通信网站，或在 SharePoint Online 租户中设置新通信网站。</span><span class="sxs-lookup"><span data-stu-id="130a4-122">Either identify an existing SharePoint communication site or provision a new one in your SharePoint Online tenant.</span></span> <span data-ttu-id="130a4-123">若要详细了解如何设置通信网站，请参阅在 [SharePoint Online](https://support.office.com/article/create-a-communication-site-in-sharepoint-online-7fb44b20-a72f-4d2c-9173-fc8f59ba50eb) 中创建通信网站并按照步骤创建通信网站。</span><span class="sxs-lookup"><span data-stu-id="130a4-123">For more information about how to provision a communication site see [Create a communication site in SharePoint Online](https://support.office.com/article/create-a-communication-site-in-sharepoint-online-7fb44b20-a72f-4d2c-9173-fc8f59ba50eb) and follow the steps to create a communication site.</span></span>

## <a name="set-permissions-for-the-site"></a><span data-ttu-id="130a4-124">设置网站的权限</span><span class="sxs-lookup"><span data-stu-id="130a4-124">Set permissions for the site</span></span>

<span data-ttu-id="130a4-125">你需要将应能够查看内容的每个人添加到 Visitors 组，以及应能够管理自定义播放列表的所有人添加到 Members 组。</span><span class="sxs-lookup"><span data-stu-id="130a4-125">You will want to add everyone who should be able to view content to the Visitors group and everyone who should be able to administer custom playlists to the Members group.</span></span> <span data-ttu-id="130a4-126">若要在用户第一次成为网站集管理员或 Owners 组的一部分时为自定义学习配置网站。</span><span class="sxs-lookup"><span data-stu-id="130a4-126">To configure the site for Custom Learning the first time the user must be either a site collection administrator or part of the Owners group.</span></span>

<span data-ttu-id="130a4-127">将 Office 365 应用的自定义学习添加到网站集。</span><span class="sxs-lookup"><span data-stu-id="130a4-127">Add Custom Learning for Office 365 App to the site collection.</span></span>

## <a name="execute-powershell-configuration-script"></a><span data-ttu-id="130a4-128">执行 PowerShell 配置脚本</span><span class="sxs-lookup"><span data-stu-id="130a4-128">Execute PowerShell Configuration Script</span></span>

<span data-ttu-id="130a4-129">包含一个 PowerShell 脚本，您需要执行该脚本来创建解决方案使用的三 `CustomLearningConfiguration.ps1` 个租户属性。 [](/sharepoint/dev/spfx/tenant-properties)</span><span class="sxs-lookup"><span data-stu-id="130a4-129">A PowerShell script `CustomLearningConfiguration.ps1` is included that you will need to execute to create three [tenant properties](/sharepoint/dev/spfx/tenant-properties) that the solution uses.</span></span> <span data-ttu-id="130a4-130">此外，该脚本在 [网站页面库中](/sharepoint/dev/spfx/web-parts/single-part-app-pages) 创建两个单部件应用程序页面，以在已知位置托管管理员和用户 Web 部件。</span><span class="sxs-lookup"><span data-stu-id="130a4-130">In addition the script creates two [single part app pages](/sharepoint/dev/spfx/web-parts/single-part-app-pages) in the site pages library to host the admin and user web parts at a known location.</span></span>

### <a name="disabling-telemetry-collection"></a><span data-ttu-id="130a4-131">禁用遥测集合</span><span class="sxs-lookup"><span data-stu-id="130a4-131">Disabling Telemetry Collection</span></span>

<span data-ttu-id="130a4-132">此解决方案的一部分包括匿名遥测跟踪选择加入，默认情况下设置为"打开"。</span><span class="sxs-lookup"><span data-stu-id="130a4-132">Part of this solution includes anonymized telemetry tracking opt in, which by default is set to on.</span></span> <span data-ttu-id="130a4-133">如果要执行手动安装，并且要关闭遥测跟踪，请更改脚本以将 $optInTelemetry 变量设置为 `CustomlearningConfiguration.ps1` $false。</span><span class="sxs-lookup"><span data-stu-id="130a4-133">If you are performing a manual install and you would like to turn telemetry tracking off, please change the `CustomlearningConfiguration.ps1` script to set the $optInTelemetry variable to $false.</span></span>

<span data-ttu-id="130a4-134">如果不执行手动安装，并且要关闭遥测跟踪，则包含单独的脚本，运行时 `TelemetryOptOut.ps1` 将禁用遥测跟踪。</span><span class="sxs-lookup"><span data-stu-id="130a4-134">If you are not performing a manual install and would like to turn telemetry tracking off, a seperate script `TelemetryOptOut.ps1` has been included that when run will disable telemetry tracking.</span></span>

## <a name="initialize-web-part-custom-configuration"></a><span data-ttu-id="130a4-135">初始化 Web 部件自定义配置</span><span class="sxs-lookup"><span data-stu-id="130a4-135">Initialize web part custom configuration</span></span>

<span data-ttu-id="130a4-136">成功运行 PowerShell 脚本后，导航到 `<YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx` 。</span><span class="sxs-lookup"><span data-stu-id="130a4-136">After the PowerShell script is successfully run, navigate to `<YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx`.</span></span> <span data-ttu-id="130a4-137">这将初始化 CustomConfig 列表项，该项设置自定义学习，供其首次使用。</span><span class="sxs-lookup"><span data-stu-id="130a4-137">This initializes the CustomConfig list item that sets up custom learning for its first use.</span></span>

<span data-ttu-id="130a4-138">配置现已完成，您可以使用自定义学习 for Office 365 继续操作。</span><span class="sxs-lookup"><span data-stu-id="130a4-138">The configuration is now complete and you can move forward with using Custom Learning for Office 365.</span></span> <span data-ttu-id="130a4-139">有关详细信息，请参阅用户文档。</span><span class="sxs-lookup"><span data-stu-id="130a4-139">Please see the user documentation for more information.</span></span>