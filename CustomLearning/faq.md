---
author: karuanag
ms.author: karuanag
title: 适用于 Office 365 解决方案的自定义学习的常见问题
ms.date: 02/10/2019
description: 适用于 Office 365 的自定义学习的常见问题信息
ms.openlocfilehash: 7da1f3da197fc298c83eac89e3455312cba7a851
ms.sourcegitcommit: 775d6807291ab263eea5ec649d9aaf1933fb41ca
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/23/2019
ms.locfileid: "32056005"
---
# <a name="frequently-asked-questions"></a><span data-ttu-id="ed6a3-103">常见问题解答</span><span class="sxs-lookup"><span data-stu-id="ed6a3-103">Frequently Asked Questions</span></span>

### <a name="1-what-are-the-requirements-for-installing-custom-learning-for-office-365-into-my-tenant-environment"></a><span data-ttu-id="ed6a3-104">1. 将适用于 Office 365 的自定义学习安装到我的租户环境中的要求是什么？</span><span class="sxs-lookup"><span data-stu-id="ed6a3-104">1. What are the requirements for installing Custom Learning for Office 365 into my tenant environment?</span></span>

- <span data-ttu-id="ed6a3-105">已启用 SharePoint Online 和通信网站。</span><span class="sxs-lookup"><span data-stu-id="ed6a3-105">SharePoint Online and Communication Sites enabled.</span></span>
- <span data-ttu-id="ed6a3-106">将设置 CLO365 的个人必须是要安装的目标租户的租户管理员。</span><span class="sxs-lookup"><span data-stu-id="ed6a3-106">The individual that will be provisioning CLO365 must be the tenant administrator of the target tenant for install.</span></span>
- <span data-ttu-id="ed6a3-107">租户的 "应用程序目录" 必须在 SharePoint 管理中心的 "应用程序" 选项中可用。</span><span class="sxs-lookup"><span data-stu-id="ed6a3-107">A tenant 'App Catalog' must be available within the 'Apps' option of the SharePoint Admin Center.</span></span>
- <span data-ttu-id="ed6a3-108">将设置 CLO365 的个人必须是目标租户中应用程序目录的网站集管理员才能安装。</span><span class="sxs-lookup"><span data-stu-id="ed6a3-108">The individual that will be provisioning CLO365 must be a site collection administrator of the app catalog in the target tenant for install.</span></span>

### <a name="2-what-languages-is-custom-learning-for-office-365-available-in"></a><span data-ttu-id="ed6a3-109">2. 适用于 Office 365 的自定义学习的语言是什么？</span><span class="sxs-lookup"><span data-stu-id="ed6a3-109">2. What languages is Custom Learning for Office 365 available in?</span></span>

<span data-ttu-id="ed6a3-110">Office 365 的自定义学习目前仅提供英文版本。</span><span class="sxs-lookup"><span data-stu-id="ed6a3-110">Custom Learning for Office 365 is currently available only in English.</span></span> <span data-ttu-id="ed6a3-111">自动端到端预配仅适用于英语租户。</span><span class="sxs-lookup"><span data-stu-id="ed6a3-111">Automatic end-to-end provisioning only works with English tenants.</span></span> <span data-ttu-id="ed6a3-112">在将来的版本中可能会添加其他语言。</span><span class="sxs-lookup"><span data-stu-id="ed6a3-112">Additional languages may be added at in future releases.</span></span>

### <a name="3-how-long-will-it-take-to-install-the-site-in-our-tenant-environment"></a><span data-ttu-id="ed6a3-113">3. 将网站安装到我们的租户环境中需要多长时间？</span><span class="sxs-lookup"><span data-stu-id="ed6a3-113">3. How long will it take to install the site in our tenant environment?</span></span>

<span data-ttu-id="ed6a3-114">根据我们的安装测试, 应花费不到15分钟的时间。</span><span class="sxs-lookup"><span data-stu-id="ed6a3-114">Based on our testing of the installation, it should take less than 15 minutes.</span></span> <span data-ttu-id="ed6a3-115">这不包括自定义网站满足您的要求所需的时间。</span><span class="sxs-lookup"><span data-stu-id="ed6a3-115">This does not include time required to customize the site to your requirements.</span></span>

### <a name="4-can-we-make-the-custom-learning-for-office-365-a-subsite-of-our-primary-sharepoint-site-collection"></a><span data-ttu-id="ed6a3-116">4. 我们主要 SharePoint 网站集的子网站是否可以为 Office 365 创建自定义学习？</span><span class="sxs-lookup"><span data-stu-id="ed6a3-116">4. Can we make the Custom learning for Office 365 a subsite of our primary SharePoint site collection?</span></span>

<span data-ttu-id="ed6a3-117">不可以。</span><span class="sxs-lookup"><span data-stu-id="ed6a3-117">No.</span></span> <span data-ttu-id="ed6a3-118">网站基于通信网站模板, 该模板始终旨在作为根网站集。</span><span class="sxs-lookup"><span data-stu-id="ed6a3-118">The site is based on a communication site template, which is always meant to be a root site collection.</span></span>

> [!NOTE]
> <span data-ttu-id="ed6a3-119">请务必考虑最终用户访问网站所需的权限。</span><span class="sxs-lookup"><span data-stu-id="ed6a3-119">It is important to consider the permissions your end users will need to access the site.</span></span> <span data-ttu-id="ed6a3-120">大多数组织已定义了安全性或用户组。</span><span class="sxs-lookup"><span data-stu-id="ed6a3-120">Most organizations have defined security or user groups.</span></span> <span data-ttu-id="ed6a3-121">准备好将适当的安全组添加到你的员工社区后, 必须将其添加到新的培训门户。</span><span class="sxs-lookup"><span data-stu-id="ed6a3-121">You must add the appropriate security groups to your new training portal once you are ready to launch it to your employee community.</span></span>

### <a name="5-i-need-to-reinstall-the-site-what-should-i-do"></a><span data-ttu-id="ed6a3-122">5. 我需要重新安装网站;我该怎么办？</span><span class="sxs-lookup"><span data-stu-id="ed6a3-122">5. I need to reinstall the site; what should I do?</span></span>

<span data-ttu-id="ed6a3-123">按照[此处](custom_provision.md)发布的安装说明进行操作。</span><span class="sxs-lookup"><span data-stu-id="ed6a3-123">Follow the installation instructions published [here](custom_provision.md).</span></span>

> [!NOTE]
> <span data-ttu-id="ed6a3-124">如果你已在之前的安装中禁用遥测, 并且要继续禁用遥测, 则需要遵循在此处禁用遥测的说明。</span><span class="sxs-lookup"><span data-stu-id="ed6a3-124">If you had disabled telemetry in your prior installation and would like to continue with telemetry disabled, you will need to follow the instructions for disabling the telemetry here.</span></span>

### <a name="6-we-made-updates-to-our-implementation-of-custom-learning-for-office-365-will-we-lose-these-updates-made-to-site-template-playlists-if-we-reinstall-the-site"></a><span data-ttu-id="ed6a3-125">6. 我们已对 Office 365 的自定义学习实施进行了更新。</span><span class="sxs-lookup"><span data-stu-id="ed6a3-125">6. We made updates to our implementation of Custom Learning for Office 365.</span></span> <span data-ttu-id="ed6a3-126">如果重新安装网站, 我们会丢失这些更新 (对网站模板, 播放列表)？</span><span class="sxs-lookup"><span data-stu-id="ed6a3-126">Will we lose these updates (made to site template, playlists) if we reinstall the site?</span></span>

<span data-ttu-id="ed6a3-127">如果通过当前安装重新安装网站, 则对单个页面和自定义播放列表的自定义将会丢失。</span><span class="sxs-lookup"><span data-stu-id="ed6a3-127">Customizations to individual pages and custom playlists will be lost if you reinstall the site over your current installation.</span></span>  