---
author: karuanag
ms.author: karuanag
title: Microsoft 365 学习途径的常见问题
ms.date: 02/10/2019
description: Microsoft 365 学习途径的常见问题信息
ms.openlocfilehash: 26d6c7140b4d387e13b907033ea53b752f5e20ea
ms.sourcegitcommit: 0077704d7edcc26eda76900115716fc5b7b1c518
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2019
ms.locfileid: "34334716"
---
# <a name="frequently-asked-questions"></a>常见问题解答

### <a name="what-are-the-requirements-for-installing-microsoft-365-learning-pathways-into-my-tenant-environment"></a>在我的租户环境中安装 Microsoft 365 学习路径的要求是什么？

- 已启用 SharePoint Online 和通信网站。
- 将设置 CLO365 的个人必须是要安装的目标租户的租户管理员。
- 租户的 "应用程序目录" 必须在 SharePoint 管理中心的 "应用程序" 选项中可用。
- 如果创建了新的应用程序目录, 则完全预配应用程序目录需要等待时间为30分钟或更多。 在创建租户应用程序目录后, 尝试直接预配 Microsoft 365 学习路径将导致学习路径解决方案的设置错误。 
- 将设置 CLO365 的个人必须是目标租户中应用程序目录的网站集管理员才能安装。

### <a name="why-is-microsoft-asking-for-tenant-permissions-when-installing-microsoft-365-learning-pathways"></a>为什么 Microsoft 在安装 Microsoft 365 学习路径时要求提供租户权限 

- SharePoint Online 设置服务使用设置学习路径 SharePoint 网站、创建网站页面以及在其租户中安装 Microsoft 365 学习路径应用程序的权限。 这是我们请求权限的唯一原因。 如果没有请求的权限, SharePoint 设置服务将无法执行可自动安装 "学习路径" 网站模板和 web 部件的命令。 

### <a name="what-are-the-implications-of-microsoft-365-learning-pathways-being-in-a-beta-preview"></a>Microsoft 365 学习路径在 Beta Preview 中有何含义？ 

Microsoft 365 学习途径目前处于 Beta Preview 中。 在评估、规划和实施 Microsoft 365 学习路径时, 请考虑以下事项:

- 与任何 Beta 解决方案一样, 我们的服务管理团队保留对服务及其组件进行更改的权利。 在我们主动解决 bug 和 UX 问题时, 您可能需要更新 Web 部件。
- 若要更新 web 部件, 你需要从 GitHub 存储库中下载它, 并将其上传到租户应用目录中。 请参阅 Microsoft 365 学习路径[自述](https://github.com/pnp/custom-learning-office-365/blob/master/README.md)文件中的 "更新解决方案" 部分。 

### <a name="what-languages-is-microsoft-365-learning-pathways-available-in"></a>中提供了哪些语言的 Microsoft 365 学习途径？

Microsoft 365 学习途径目前仅提供英文版本。 自动端到端预配仅适用于英语租户。 我们计划在 CY19 Q3 中推出以下九种语言的多语言支持: 

- 中文（简体） 
- 荷兰语（荷兰） 
- 法语  
- 德语 
- 意大利语（意大利） 
- 日语（日本）  
- 葡萄牙语（巴西） 
- 俄语 (俄语)  
- 西班牙语 

### <a name="how-long-will-it-take-to-install-the-site-in-our-tenant-environment"></a>在我们的租户环境中安装网站需要多长时间？

根据我们的安装测试, 应花费不到15分钟的时间。 这不包括自定义网站满足您的要求所需的时间。

### <a name="is-microsoft-365-learning-pathways-an-open-source-solution-and-what-are-the-implications"></a>Microsoft 365 学习与开放源代码解决方案的路径以及有什么影响？

Microsoft 365 的学习途径是开放源代码软件 (OSS) 解决方案, 因此在 OSS 中附带了一组优点和注意事项 germane:

#### <a name="benefits"></a>优点 
- **Microsoft 365 学习途径是一个免费的解决方案:** 客户可以在其租户中安装解决方案, 对其进行自定义并使其可供最终用户使用
- **OSS 支持快速开发和协作:** 所有开放源代码解决方案都可供广泛的参与者社区使用。  Microsoft 致力于促进创新的这一方法。  为确保我们提供的体验能够受益于我们最广泛的客户集, 我们的核心服务管理团队将保留用于确定将哪些内容合并到官方内部版本的权利。  
- **OSS 实现与合作伙伴的协作:** Microsoft 正在与多个学习合作伙伴合作, 以支持其未来扩展和对 Microsoft 365 学习途径的贡献。 我们将提供详细信息, 因为这些计划将成为最终完成。 
    
#### <a name="implications"></a>方面
- **OSS 不是一个商业产品:** 商业产品包括更新和修补, 并包含在收费支持合同中。 虽然 Microsoft 目前提供了文档、更新和修补 Microsoft 365 学习途径, 但它基于改进此特定业务方案的承诺。 我们的计划是继续投资学习途径, 但客户应注意, 我们的服务管理团队可能会在将来更改策略。 以后对 Microsoft 365 学习路径所做的任何更改都将提前生效。 
- **作为 OSS, 通过 GitHub 上的联机问题列表支持 microsoft 365 学习路径**: microsoft 365 学习通道不受任何现有 Microsoft 支持合同的覆盖。 提交的问题由 Microsoft 365 学习路径服务所有者和社区进行会审。 问题解决服务级别与付费 Microsoft 支持合同的级别不相同。  

### <a name="can-we-make-the-microsoft-365-learning-pathways-a-subsite-of-our-primary-sharepoint-site-collection"></a>我们是否可以让 Microsoft 365 学习路径成为我们主要 SharePoint 网站集的子网站？

否。 网站基于通信网站模板, 该模板始终旨在作为根网站集。

> [!NOTE]
> 请务必考虑最终用户访问网站所需的权限。 大多数组织已定义了安全性或用户组。 准备好将适当的安全组添加到你的员工社区后, 必须将其添加到新的培训门户。

### <a name="i-need-to-reinstall-the-site-what-should-i-do"></a>我需要重新安装网站;我该怎么办？

按照[此处](custom_provision.md)发布的安装说明进行操作。

> [!NOTE]
> 如果你已在之前的安装中禁用遥测, 并且要继续禁用遥测, 则需要遵循在此处禁用遥测的说明。

### <a name="we-made-updates-to-our-implementation-of-microsoft-365-learning-pathways-will-we-lose-these-updates-made-to-site-template-playlists-if-we-reinstall-the-site"></a>我们已对 Microsoft 365 学习途径的实施进行了更新。 如果重新安装网站, 我们会丢失这些更新 (对网站模板, 播放列表)？

如果通过当前安装重新安装网站, 则对单个页面和自定义播放列表的自定义将会丢失。  