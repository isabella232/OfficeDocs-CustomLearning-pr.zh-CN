---
title: Microsoft 365学习路径常见问题解答
author: karuanag
ms.author: karuanag
manager: alexb
ms.date: 02/10/2019
description: 有关学习路径的Microsoft 365常见问题信息
ms.service: sharepoint-online
ms.topic: article
ms.openlocfilehash: f24f16455ba41724d300d038a01dc04c2170dc4a
ms.sourcegitcommit: 33acfc2149de89e8375b064b2223cae505d2a102
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52575917"
---
# <a name="frequently-asked-questions"></a>常见问题解答

### <a name="i-recently-saw-a-blog-post-that-custom-learning-for-office-365-is-being-renamed-to-microsoft-365-learning-pathways-are-there-other-changes-being-added-to-the-solution-as-part-of-the-renaming-effort-should-i-update-the-solution-in-my-organization"></a>我最近看到一篇博客文章，Office 365自定义学习方式Microsoft 365学习路径。 是否正在将其他更改作为重命名工作的一部分添加到解决方案中？ 我应在我的组织中更新解决方案吗？

学习Microsoft 365路径发布是一项重新品牌打造工作，致力于更改解决方案的名称，以与品牌Microsoft 365一致。 如果你有自定义学习 for Office 365当前在组织中成功运行，则此时不需要更新解决方案。  

### <a name="what-are-the-requirements-for-installing-microsoft-365-learning-pathways-into-my-tenant-environment"></a>将学习路径Microsoft 365我的租户环境中有什么要求？

- 启用了 SharePoint Online 和通信网站。
- 要预配的用户必须为目标租户的租户管理员进行安装。
- 租户"应用程序目录"必须在管理中心的"应用程序"选项SharePoint提供。
- 如果创建了新的应用程序目录，则完全设置应用程序目录需要 30 分钟或更多的等待时间。 尝试在创建Microsoft 365应用程序目录后直接预配学习路径将导致学习路径解决方案设置错误。 
- 将预配的用户必须是目标租户中应用程序目录的网站集管理员才能安装。

### <a name="why-is-microsoft-asking-for-tenant-permissions-when-installing-microsoft-365-learning-pathways"></a>为什么 Microsoft 在安装学习路径时Microsoft 365租户权限 

- SharePoint Online Provisioning Service 使用权限预配学习路径 SharePoint 网站、创建网站页面，以及在其租户中安装 Microsoft 365 学习路径应用程序。 这是请求权限的唯一原因。 如果没有请求的权限，SharePoint服务将无法执行自动安装学习路径网站模板和 Web 部件的命令。 

### <a name="what-are-the-implications-of-microsoft-365-learning-pathways-being-in-a-beta-preview"></a>Beta 预览版Microsoft 365学习路径的含义是什么？ 

Microsoft 365 Beta 预览版中目前提供学习路径。 在评估、规划和实施学习路径时，请考虑Microsoft 365以下事项：

- 与任何 Beta 解决方案一样，我们的服务管理团队保留对服务及其组件进行更改的权利。 在主动解决 Bug 和 UX 问题时，可能需要更新 WebPart。
- 若要更新 Web 部件，你需要从我们的 GitHub 下载它并将其上传到你的租户应用程序目录。 请参阅"学习路径自述文件"Microsoft 365"更新[解决方案"](https://github.com/pnp/custom-learning-office-365/blob/master/README.md)部分。 

### <a name="what-languages-is-microsoft-365-learning-pathways-available-in"></a>学习路径Microsoft 365哪些语言？

Microsoft 365学习路径目前仅提供英文版。 端到端自动预配仅适用于英语租户。 我们计划在 2020 年第二季度推出对以下语言的多语言支持。 

- 中文(简体) 
- 法语  
- 德语 
- 意大利语（意大利） 
- 日语（日本）  
- 葡萄牙语（巴西） 
- 俄语 (俄语)   
- 西班牙语 

> 对荷兰语的支持不会包含在即将推出的多语言学习路径支持版本中。 我们今后将继续评估新的语言选项。

### <a name="how-long-will-it-take-to-install-the-site-in-our-tenant-environment"></a>在租户环境中安装网站需要多久？

根据我们测试的安装，它应少于 15 分钟。 这不包括根据你的要求自定义网站所需的时间。

### <a name="is-microsoft-365-learning-pathways-an-open-source-solution-and-what-are-the-implications"></a>Microsoft 365学习路径是开放源代码解决方案吗？

Microsoft 365学习路径是 OSS (解决方案中的) 软件，因此，OSS 具有一组优点和注意事项：

#### <a name="benefits"></a>优点 
- **Microsoft 365学习路径是一种免费解决方案：** 客户可以在租户中安装解决方案、自定义解决方案并提供给最终用户
- **OSS 支持快速开发和协作：**  所有开放源代码解决方案都适用于广泛的参与者社区。  Microsoft 致力于此推动创新的方法。  为了确保我们提供的体验有利于我们最广大的客户，我们的核心服务管理团队将保留确定哪些贡献合并到正式内部版本的权利。  
- **OSS 支持与合作伙伴进行协作：** Microsoft 正在与多个学习合作伙伴合作，以支持他们为将来扩展和为学习路径Microsoft 365贡献。 随着这些计划的完成，我们将提供更多信息。 
    
#### <a name="implications"></a>含义
- **OSS 不是商业提供的产品：** 商业产品包括更新和修补，包括在基于费用的支持合同内。 虽然 Microsoft 目前提供文档、更新和修补Microsoft 365学习路径，但基于我们对改进此特定业务方案的承诺。 我们的计划是继续投资学习路径，请注意，我们的服务管理团队将来可能会更改策略。 对学习Microsoft 365的任何未来更改都将在生效之前传达。 
- **作为 OSS，Microsoft 365 GitHub** 上的联机问题列表支持这些学习路径：Microsoft 365任何现有 Microsoft 支持合同都未涵盖这些学习路径。 提交的问题由Microsoft 365服务所有者和社区进行会审。 问题解决服务级别与付费 Microsoft 支持合同不在同一级别。  

### <a name="can-we-make-the-microsoft-365-learning-pathways-a-subsite-of-our-primary-sharepoint-site-collection"></a>我们能否将Microsoft 365路径作为我们主要网站集的SharePoint网站？

不正确。 该网站基于通信网站模板，该模板始终作为根网站集。

> [!NOTE]
> 必须考虑最终用户访问网站所需的权限。 大多数组织已定义安全组或用户组。 准备好将其启动到员工社区后，必须将相应的安全组添加到新培训门户。

### <a name="i-need-to-reinstall-the-site-what-should-i-do"></a>我需要重新安装站点;我应该做什么？

按照此处发布的安装 [说明操作](custom_provision.md)。

> [!NOTE]
> 如果你在以前的安装中禁用了遥测，并且希望继续禁用遥测，则需要按照此处禁用遥测的说明操作。

### <a name="we-made-updates-to-our-implementation-of-microsoft-365-learning-pathways-will-we-lose-these-updates-made-to-site-template-playlists-if-we-reinstall-the-site"></a>我们对实现学习路径Microsoft 365更新。 如果重新安装网站， (对网站模板、播放列表) 丢失这些更新吗？

如果在当前安装过程中重新安装网站，则单个页面和自定义播放列表的自定义项将丢失。  
