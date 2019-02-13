---
author: karuanag
ms.author: karuanag
title: 用于 Office 365 解决方案的自定义学习的常见问题
ms.date: 02/10/2019
description: 自定义学习问题信息的 Office 365 常见问题
ms.openlocfilehash: d8b5104e8feeaa4e70296f61594233b27363481b
ms.sourcegitcommit: f93a6a691331515ba10f4d43b491928ec268f0ec
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/12/2019
ms.locfileid: "29952593"
---
# <a name="frequently-asked-questions"></a><span data-ttu-id="e0e50-103">常见问题解答</span><span class="sxs-lookup"><span data-stu-id="e0e50-103">Frequently Asked Questions</span></span>

### <a name="1-what-are-the-requirements-for-installing-custom-learning-for-office-365-into-my-tenant-environment"></a><span data-ttu-id="e0e50-104">1.什么是 Office 365 的自定义学习安装到我的租户环境的要求？</span><span class="sxs-lookup"><span data-stu-id="e0e50-104">1. What are the requirements for installing Custom Learning for Office 365 into my tenant environment?</span></span>

- <span data-ttu-id="e0e50-105">SharePoint Online 和通信网站启用。</span><span class="sxs-lookup"><span data-stu-id="e0e50-105">SharePoint Online and Communication Sites enabled.</span></span>
- <span data-ttu-id="e0e50-106">将资源调配 CLO365 个人必须安装目标租户的租户管理员。</span><span class="sxs-lookup"><span data-stu-id="e0e50-106">The individual that will be provisioning CLO365 must be the tenant administrator of the target tenant for install.</span></span>
- <span data-ttu-id="e0e50-107">必须在 SharePoint 管理中心的应用程序选项中的可用租户应用程序目录。</span><span class="sxs-lookup"><span data-stu-id="e0e50-107">A tenant 'App Catalog' must be available within the 'Apps' option of the SharePoint Admin Center.</span></span>
- <span data-ttu-id="e0e50-108">将资源调配 CLO365 个人必须安装为目标租户中应用程序目录网站集管理员。</span><span class="sxs-lookup"><span data-stu-id="e0e50-108">The individual that will be provisioning CLO365 must be a site collection administrator of the app catalog in the target tenant for install.</span></span>

### <a name="2-what-languages-is-custom-learning-for-office-365-available-in"></a><span data-ttu-id="e0e50-109">2.何种语言是 Office 365 的自定义学习中提供？</span><span class="sxs-lookup"><span data-stu-id="e0e50-109">2. What languages is Custom Learning for Office 365 available in?</span></span>

<span data-ttu-id="e0e50-p101">自定义 Office 365 学习是当前仅提供英文版。自动端到端设置仅适用于英文租户。版本可能在未来添加的其他语言。</span><span class="sxs-lookup"><span data-stu-id="e0e50-p101">Custom Learning for Office 365 is currently available only in English. Automatic end-to-end provisioning only works with English tenants. Additional languages may be added at in future releases.</span></span>

### <a name="3-how-long-will-it-take-to-install-the-site-in-our-tenant-environment"></a><span data-ttu-id="e0e50-113">3.我们租户环境中安装网站将需要多长时间？</span><span class="sxs-lookup"><span data-stu-id="e0e50-113">3. How long will it take to install the site in our tenant environment?</span></span>

<span data-ttu-id="e0e50-p102">根据我们测试安装的它应采取不超过 15 分钟。这不包括自定义网站，您的要求所需时间。</span><span class="sxs-lookup"><span data-stu-id="e0e50-p102">Based on our testing of the installation, it should take less than 15 minutes. This does not include time required to customize the site to your requirements.</span></span>

### <a name="4-can-we-make-the-custom-learning-for-office-365-a-subsite-of-our-primary-sharepoint-site-collection"></a><span data-ttu-id="e0e50-116">4.可以使自定义 Office 365 学习我们主的 SharePoint 网站集的子网站？</span><span class="sxs-lookup"><span data-stu-id="e0e50-116">4. Can we make the Custom learning for Office 365 a subsite of our primary SharePoint site collection?</span></span>

<span data-ttu-id="e0e50-p103">不。网站基于通信网站模板，旨在始终是根网站集。</span><span class="sxs-lookup"><span data-stu-id="e0e50-p103">No. The site is based on a communication site template, which is always meant to be a root site collection.</span></span>

> [!NOTE]
> <span data-ttu-id="e0e50-p104">请务必考虑您的最终用户将需要访问网站的权限。大多数组织已定义安全或用户组。后即可启动与员工社区，您必须将适当的安全组添加到新的培训门户。</span><span class="sxs-lookup"><span data-stu-id="e0e50-p104">It is important to consider the permissions your end users will need to access the site. Most organizations have defined security or user groups. You must add the appropriate security groups to your new training portal once you are ready to launch it to your employee community.</span></span>

### <a name="5-i-need-to-reinstall-the-site-what-should-i-do"></a><span data-ttu-id="e0e50-122">5.我需要重新安装网站;应该怎样做？</span><span class="sxs-lookup"><span data-stu-id="e0e50-122">5. I need to reinstall the site; what should I do?</span></span>

<span data-ttu-id="e0e50-123">按照安装说明发布[此处](installsitepackage.md)。</span><span class="sxs-lookup"><span data-stu-id="e0e50-123">Follow the installation instructions published [here](installsitepackage.md).</span></span>

> [!NOTE]
> <span data-ttu-id="e0e50-124">如果您具有您以前的安装中禁用遥测，并且希望继续使用遥测禁用您需要按照用于禁用的遥测数据的说明。</span><span class="sxs-lookup"><span data-stu-id="e0e50-124">If you had disabled telemetry in your prior installation and would like to continue with telemetry disabled, you will need to follow the instructions for disabling the telemetry here.</span></span>

### <a name="6-we-made-updates-to-our-implementation-of-custom-learning-for-office-365-will-we-lose-these-updates-made-to-site-template-playlists-if-we-reinstall-the-site"></a><span data-ttu-id="e0e50-p105">6.我们对我们的自定义学习 for Office 365 的实现进行了更新。如果我们重新安装网站，我们将丢失 （对网站模板，播放列表） 这些更新？</span><span class="sxs-lookup"><span data-stu-id="e0e50-p105">6. We made updates to our implementation of Custom Learning for Office 365. Will we lose these updates (made to site template, playlists) if we reinstall the site?</span></span>

<span data-ttu-id="e0e50-127">如果您重新安装通过当前安装的网站，单个页面和自定义播放列表的自定义项都将丢失。</span><span class="sxs-lookup"><span data-stu-id="e0e50-127">Customizations to individual pages and custom playlists will be lost if you reinstall the site over your current installation.</span></span>  