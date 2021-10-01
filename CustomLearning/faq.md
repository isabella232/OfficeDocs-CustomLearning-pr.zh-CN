---
title: Microsoft 365学习路径常见问题解答
author: karuanag
ms.author: karuanag
manager: alexb
ms.date: 02/10/2019
description: 有关学习路径的Microsoft 365常见问题信息
ms.service: sharepoint-online
ms.topic: article
ms.openlocfilehash: 82a7e777490e13fde6fef5add40beee417050027
ms.sourcegitcommit: d05381fc4a58cf2949773d73877bacc5ef3a7ca6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/01/2021
ms.locfileid: "60048719"
---
# <a name="frequently-asked-questions"></a>常见问题解答

## <a name="what-are-the-requirements-for-installing-microsoft-365-learning-pathways-into-my-tenant-environment"></a>将学习路径Microsoft 365我的租户环境中有什么要求？

- 启用了 SharePoint Online 和通信网站。
- 要预配学习路径Microsoft 365必须是要安装的目标租户的租户管理员。
- 租户"应用程序目录"必须在管理中心的"应用程序"SharePoint可用。
- 如果创建了新的应用程序目录，则完全设置应用程序目录需要 30 分钟或更多的等待时间。 尝试在创建Microsoft 365应用程序目录后直接预配学习路径将导致学习路径解决方案的预配错误。
- 要预配学习路径Microsoft 365必须是目标租户中应用程序目录的网站集管理员才能安装。

## <a name="why-is-microsoft-asking-for-tenant-permissions-when-installing-microsoft-365-learning-pathways"></a>为什么 Microsoft 在安装学习路径时Microsoft 365租户权限？

SharePoint Online Provisioning Service 使用权限预配 Learning 路径 SharePoint 网站、创建网站页面，以及在其租户中安装 Microsoft 365 学习路径应用程序。 这是请求权限的唯一原因。 如果没有请求的权限，SharePoint服务将无法执行自动安装学习路径网站模板和 Web 部件的命令。
![权限请求的屏幕截图](media/faqs-permissions-request-screenshot.png "权限请求") 如果对此级别的访问权限仍有顾虑，可以授予权限并部署感兴趣的任何网站模板，然后立即删除 Azure 应用商店中向应用授予 [的权限](https://myapps.microsoft.com)。

## <a name="how-long-will-it-take-to-install-the-site-in-our-tenant-environment"></a>在租户环境中安装网站需要多久？

它应少于 15 分钟。 这不包括根据你的要求自定义网站所需的时间。

## <a name="is-microsoft-365-learning-pathways-an-open-source-solution-and-what-are-the-implications"></a>Microsoft 365学习路径是开放源代码解决方案吗？

Microsoft 365学习路径是 OSS (解决方案) 开源软件，因此，OSS 具有一组优点和注意事项：

### <a name="benefits"></a>优点 

- **Microsoft 365学习路径是一种免费解决方案：** 客户可以在其租户中安装、自定义解决方案，并提供给最终用户使用。
- **OSS 支持快速开发和协作：** 所有开放源代码解决方案都适用于广泛的参与者社区。 Microsoft 致力于此推动创新的方法。 为了确保我们提供的体验有利于我们最广大的客户，我们的核心服务管理团队将保留确定哪些贡献合并到正式内部版本的权利。  
- **OSS 支持与合作伙伴进行协作：** Microsoft 正在与多个学习合作伙伴合作，以支持他们为将来扩展和为学习路径Microsoft 365贡献。 随着这些计划的完成，我们将提供更多信息。

### <a name="implications"></a>含义

- **OSS 不是商业提供的产品：** 商业产品包括更新和修补，包括在基于费用的支持合同内。 虽然 Microsoft 目前提供文档、更新和修补Microsoft 365学习路径，但它基于我们对改进此特定业务方案的承诺。 尽管我们的计划将继续投资学习路径，但请注意，我们的服务管理团队将来可能会更改策略。 在生效之前Microsoft 365对学习路径的任何未来更改都会得到传达。
- **作为 OSS，Microsoft 365 GitHub** 上的联机问题列表支持这些学习路径：Microsoft 365任何现有 Microsoft 支持合同都未涵盖这些学习路径。 提交的问题由服务Microsoft 365和社区按学习路径分类。 问题解决服务级别与付费 Microsoft 支持合同不在同一级别。  

### <a name="can-we-make-the-microsoft-365-learning-pathways-a-sub-site-of-our-primary-sharepoint-site-collection"></a>我们能否将Microsoft 365路径作为主网站集的子SharePoint网站？

不需要。 该网站基于通信网站模板，该模板始终是根网站集。

> [!NOTE]
> 必须考虑最终用户访问网站所需的权限。 大多数组织已定义安全组或用户组。 准备好将其启动到员工社区后，必须将相应的安全组添加到新培训门户。

### <a name="i-need-to-reinstall-the-site-what-should-i-do"></a>我需要重新安装站点;我应该做什么？

按照此处发布的安装 [说明操作](custom_provision.md)。

> [!NOTE]
> 如果你在以前的安装中禁用了遥测，并且希望继续禁用遥测，则需要按照此处有关禁用遥测 [的说明操作](https://github.com/pnp/custom-learning-office-365/blob/a7168c97a76e0b4122e3ddfc530f6a10c724c3e1/installation/README.md)。

### <a name="we-made-updates-to-our-implementation-of-microsoft-365-learning-pathways-will-we-lose-these-updates-made-to-site-template-playlists-if-we-reinstall-the-site"></a>我们对实现学习路径Microsoft 365更新。 如果重新安装网站， (对网站模板、播放列表) 丢失这些更新吗？

如果在当前安装过程中重新安装网站，则单个页面和自定义播放列表的自定义项将丢失。  
