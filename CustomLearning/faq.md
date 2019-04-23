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
# <a name="frequently-asked-questions"></a>常见问题解答

### <a name="1-what-are-the-requirements-for-installing-custom-learning-for-office-365-into-my-tenant-environment"></a>1. 将适用于 Office 365 的自定义学习安装到我的租户环境中的要求是什么？

- 已启用 SharePoint Online 和通信网站。
- 将设置 CLO365 的个人必须是要安装的目标租户的租户管理员。
- 租户的 "应用程序目录" 必须在 SharePoint 管理中心的 "应用程序" 选项中可用。
- 将设置 CLO365 的个人必须是目标租户中应用程序目录的网站集管理员才能安装。

### <a name="2-what-languages-is-custom-learning-for-office-365-available-in"></a>2. 适用于 Office 365 的自定义学习的语言是什么？

Office 365 的自定义学习目前仅提供英文版本。 自动端到端预配仅适用于英语租户。 在将来的版本中可能会添加其他语言。

### <a name="3-how-long-will-it-take-to-install-the-site-in-our-tenant-environment"></a>3. 将网站安装到我们的租户环境中需要多长时间？

根据我们的安装测试, 应花费不到15分钟的时间。 这不包括自定义网站满足您的要求所需的时间。

### <a name="4-can-we-make-the-custom-learning-for-office-365-a-subsite-of-our-primary-sharepoint-site-collection"></a>4. 我们主要 SharePoint 网站集的子网站是否可以为 Office 365 创建自定义学习？

不可以。 网站基于通信网站模板, 该模板始终旨在作为根网站集。

> [!NOTE]
> 请务必考虑最终用户访问网站所需的权限。 大多数组织已定义了安全性或用户组。 准备好将适当的安全组添加到你的员工社区后, 必须将其添加到新的培训门户。

### <a name="5-i-need-to-reinstall-the-site-what-should-i-do"></a>5. 我需要重新安装网站;我该怎么办？

按照[此处](custom_provision.md)发布的安装说明进行操作。

> [!NOTE]
> 如果你已在之前的安装中禁用遥测, 并且要继续禁用遥测, 则需要遵循在此处禁用遥测的说明。

### <a name="6-we-made-updates-to-our-implementation-of-custom-learning-for-office-365-will-we-lose-these-updates-made-to-site-template-playlists-if-we-reinstall-the-site"></a>6. 我们已对 Office 365 的自定义学习实施进行了更新。 如果重新安装网站, 我们会丢失这些更新 (对网站模板, 播放列表)？

如果通过当前安装重新安装网站, 则对单个页面和自定义播放列表的自定义将会丢失。  