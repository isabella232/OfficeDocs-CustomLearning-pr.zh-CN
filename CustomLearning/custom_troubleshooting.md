---
author: pkrebs
ms.author: pkrebs
title: Microsoft 365 学习路径故障排除
ms.date: 02/10/2019
description: 了解如何解决 Microsoft 365 学习路径问题
ms.service: sharepoint-online
manager: bpardi
ms.topic: article
audience: admin
ms.openlocfilehash: 7190688d574042c8a1b8dfb67c8b246dfbf8c927
ms.sourcegitcommit: 97e175e5ff5b6a9e0274d5ec9b39fdf7e18eb387
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/25/2021
ms.locfileid: "52000298"
---
# <a name="troubleshoot-microsoft-365-learning-pathways"></a>Microsoft 365 学习路径疑难解答

以下是有关 Microsoft 365 学习路径或 SharePoint Online 预配服务中可能存在的问题的疑难解答提示。

## <a name="how-to-know-if-you-have-tenant-admin-permissions"></a>如何知道您是否具有租户管理员权限

登录 SharePoint Online 预配服务并预配自定义学习需要租户管理员权限。 如果遇到 SharePoint Online 预配服务的登录问题，请确保已分配有全局管理员角色。 自定义学习解决方案需要租户管理员权限，也称为 Office 365 全局管理员角色。 下面是如何确定是否分配了全局管理员角色。

1.  登录到 Office.com。
2.  单击 **"管理员"**
3.  在 **"用户"** 下，选择 **"活动用户"**
4.  搜索你的姓名
5.  在搜索结果中单击你的姓名。 应看到角色的全局管理员。
![列出角色以及许可证、组成员身份和其他信息的示例页面。](media/cg-globaladminrole.png)

### <a name="if-you-dont-have-the-global-administrator-role"></a>如果你没有全局管理员角色
- 在组织中查找全局管理员，让此人登录该服务或让他们分配全局管理员角色。

## <a name="tenant-app-catalog-troubleshooting"></a>租户应用程序目录疑难解答
自定义学习需要在目标租户中预配应用程序目录。 创建应用程序目录需要全局管理员权限。 以下是常见应用程序目录问题的疑难解答步骤：

### <a name="how-to-know-if-you-have-a-tenant-app-catalog"></a>如何知道您是否具有租户应用程序目录 
对于初学者，请确保你拥有全局管理员权限。 请参阅上述租户管理员权限的步骤。

1. From Office 365， click **Admin**， click the expand arrow >， click **Show all**  >  **Admin centers**  >  **SharePoint**.
2. 单击 **经典管理 SharePoint 中心**  >  **应用程序**  >  **应用程序目录**。
3. 在 **"应用程序**"下，应看到标题为"分发 **SharePoint 应用程序"的磁贴**。 如果你看到此磁贴，则你有一个租户应用程序目录。 请参阅 **下面的如何确保你是网站集合...** 部分。 如果看不到磁贴，则需要为租户创建租户应用目录。 请参阅 **下面的如何创建租户应用程序目录** 部分。

### <a name="how-to-ensure-you-are-a-site-collection-owner-on-the-tenant-app-catalog"></a>如何确保你是租户应用程序目录中的网站集所有者 
若要预配 Microsoft 365 学习路径，你需要是租户应用目录中的网站集所有者。 下面将了解如何确定您是否为所有者。

1. From Office 365， click **Admin**， click the expand arrow >， click **Show all**  >  **Admin centers**  >  **SharePoint**.
2. 单击 **"经典管理 SharePoint 中心**"，然后选择 **应用程序目录**。
3. 选择 **"** 所有者"，然后确保您是网站集所有者。 它应如下所示。
!["管理管理员"页。](media/cg-sitecollectionowner.png)

### <a name="how-to-create-a-tenant-app-catalog-if-one-doesnt-exists"></a>如何创建租户应用程序目录（如果不存在） 
1. 使用 SharePoint Online 管理员帐户登录 Office 365。
2. 单击“**管理员**”。
3. 在"**管理中心"下**，单击 **"SharePoint"。** 
4. 单击 **应用程序**  >  **应用程序目录**。
5. 单击 **"新建应用程序目录网站"，** 然后单击"确定 **"。** 
6.  输入应用程序目录的信息。 您可能需要包括多个管理员。 下面显示了一个示例。  
![用于输入新应用程序目录信息的表单。](media/cg-appcatalogfinish.png)

7.  就是这样。 已完成。 但在设置自定义学习之前，你需要等待至少 30 分钟，以确保应用程序目录创建完成。 

> [!IMPORTANT]
> 在创建租户应用程序目录后至少等待 30 分钟，然后再预配自定义学习。 这将确保应用程序目录预配过程在 SharePoint 中完成。 