---
author: pkrebs
ms.author: pkrebs
title: 自定义学习疑难解答
ms.date: 02/10/2019
description: 了解如何排除自定义学习故障
ms.openlocfilehash: 7cbd049d4794d14f9e8cc26fd0db5f444812d688
ms.sourcegitcommit: 775d6807291ab263eea5ec649d9aaf1933fb41ca
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/23/2019
ms.locfileid: "32055078"
---
# <a name="troubleshoot-custom-learning"></a>自定义学习疑难解答

下面是针对 Office 365 或 SharePoint Online 设置服务的自定义学习功能时可能出现的问题的故障排除提示。

## <a name="how-to-know-if-you-have-tenant-admin-permissions"></a>如何知道你是否拥有租户管理员权限

登录到 SharePoint Online 设置服务并设置自定义学习需要租户管理员权限。 如果您在使用 SharePoint Online 设置服务时遇到登录问题, 请确保已为您分配全局管理员角色。 自定义学习解决方案需要租户管理员权限, 否则称为 Office 365 全局管理员角色。 下面介绍了如何确定是否已向你分配全局管理员角色。

1.  登录到 Office.com。
2.  单击 "**管理**"
3.  在 "**用户**" 下, 选择 "**活动用户**"
4.  搜索您的姓名
5.  在搜索结果中单击您的姓名。 您应看到您的角色的全局管理员。

![cg-globaladminrole](media/cg-globaladminrole.png)

### <a name="if-you-dont-have-the-global-administrator-role"></a>如果你没有全局管理员角色
- 在您的组织中查找全局管理员, 并让该用户登录到该服务, 或让其为您分配全局管理员角色。

## <a name="tenant-app-catalog-troubleshooting"></a>租户应用程序目录故障排除
自定义学习要求在目标租户中预配应用程序目录。 创建应用程序目录需要全局管理员权限。 下面是常见应用程序目录问题的故障排除步骤:

### <a name="how-to-know-if-you-have-a-tenant-app-catalog"></a>如何知道你是否拥有租户应用目录 
对于初学者, 请确保您具有全局管理员权限。 请参阅上述租户管理员权限的步骤。

1. 从 Office 365 中, 单击 "**管理**", 单击 "展开" 箭头 >, 单击 "**显示所有** > **管理中心** > **SharePoint**"。
2. 单击 "**经典管理 SharePoint 中心** > **应用** > **程序目录**"。
3. 在 "**应用程序**" 下, 应看到一个标有 "**分布 SharePoint 相关应用程序**" 的磁贴 如果您看到磁贴, 则您有租户应用程序目录。 请参阅下面的**如何确保你是网站 Colllection ...** 部分。 如果看不到磁贴, 你将需要为租户创建租户应用目录。 请参阅下面的**如何创建租户应用目录**部分。

### <a name="how-to-ensure-you-are-a-site-collection-owner-on-the-tenant-app-catalog"></a>如何确保你是租户应用程序目录上的网站集所有者 
若要为 Office 365 预配自定义学习, 您需要是租户应用程序目录上的网站集所有者。 如果你是所有者, 下面介绍了如何 determin。

1. 从 Office 365 中, 单击 "**管理**", 单击 "展开" 箭头 >, 单击 "**显示所有** > **管理中心** > **SharePoint**"。
2. 单击 "**经典管理 SharePoint 中心**", 然后选择 "**应用程序目录**"。
3. 选择 "**所有者**", 然后确保您是网站集所有者。 它应类似于以下内容。
 
![cg-sitecollectionowner](media/cg-sitecollectionowner.png)

### <a name="how-to-create-a-tenant-app-catalog-if-one-doesnt-exists"></a>如何创建租户应用程序目录 (如果不存在) 
1. 使用您的 SharePoint Online 管理员帐户登录到 Office 365。
2. 单击“**管理员**”。
3. 在 "**管理中心**" 下, 单击 " **SharePoint**"。 
4. 单击 "**应用** > "**应用程序目录**。
5. 单击 "**新建应用程序目录网站**", 然后单击 **"确定"**。 
6.  输入应用程序目录的信息。 您可能想要包含多个管理员。 下面显示了一个示例。  

![cg-appcatalogfinish](media/cg-appcatalogfinish.png)

7.  就是这样。 已经完成。 但在迁移到预配自定义学习之前, 至少需要等待30分钟, 才能确保应用程序目录创建已完成。 

> [!IMPORTANT]
> 创建租户应用程序目录后至少等待30分钟, 然后再设置自定义学习。 这可确保应用程序目录设置过程在 SharePoint 中完成。 