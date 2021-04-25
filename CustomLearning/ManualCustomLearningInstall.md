---
author: pkrebs
ms.author: pkrebs
title: 手动安装学习路径
ms.date: 02/18/2019
manager: bpardi
description: 手动安装学习路径
ms.service: sharepoint-online
ms.openlocfilehash: 7dd43e7ed66b7a8fdcd40d76d9d2bcb9403ad4bb
ms.sourcegitcommit: 97e175e5ff5b6a9e0274d5ec9b39fdf7e18eb387
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/25/2021
ms.locfileid: "51999208"
---
# <a name="manually-installing-and-configuring-custom-learning-for-office-365"></a>手动安装和配置 Office 365 的自定义学习

Microsoft 自定义学习Web 部件 [使用 SharePoint 框架](/sharepoint/dev/spfx/sharepoint-framework-overview) 版本 1.7.1 生成。

若要手动安装和配置 Web 部件和网站集，需要完成以下步骤：

1. 验证是否满足所有先决条件。
1. 在 Office 365 租户应用程序目录中安装 customlearning.sppkg 文件。
1. 设置/标识新式通信网站，以用作 Office 365 自定义学习主网站。
1. 执行 PowerShell 脚本，该脚本使用自定义学习所依赖的适当项目配置租户。
1. 导航到 CustomLearningAdmin.aspx 网站页面，以加载管理员 Web 部件以初始化自定义内容配置。

## <a name="prerequisites"></a>先决条件

你必须已设置和配置租户范围的应用程序目录。 请参阅 [设置 Office 365 租户](/sharepoint/dev/spfx/set-up-your-developer-tenant#create-app-catalog-site) 并按照创建应用程序目录网站部分操作。 如果租户范围的应用程序目录已预配，则需要访问具有将程序包上载到该帐户权限的帐户才能完成此设置过程。 通常，此帐户具有 SharePoint 管理员角色。 如果具有该角色的帐户不起作用，请转到 SharePoint 管理中心并查找应用程序目录网站集的网站集管理员，并作为网站集管理员之一登录，或者向网站集管理员添加失败的 SharePoint 管理员帐户。 你还需要访问作为 SharePoint 租户管理员的帐户。

## <a name="upload-the-web-part-to-the-tenant-app-catalog"></a>将 Web 部件上载到租户应用程序目录

若要设置 Office 365 的自定义学习，您需要将 customlearning.sppkg 文件上载到租户范围的应用程序目录并部署它。 有关如何 [将应用程序添加到](/sharepoint/use-app-catalog) 应用程序目录的详细说明，请参阅使用应用程序目录为 SharePoint Online 环境提供自定义业务应用程序。

## <a name="provisionidentify-modern-communication-site"></a>预配/识别新式通信网站

确定现有 SharePoint 通信网站，或在 SharePoint Online 租户中设置新通信网站。 若要详细了解如何设置通信网站，请参阅在 [SharePoint Online](https://support.office.com/article/create-a-communication-site-in-sharepoint-online-7fb44b20-a72f-4d2c-9173-fc8f59ba50eb) 中创建通信网站并按照步骤创建通信网站。

## <a name="set-permissions-for-the-site"></a>设置网站的权限

你需要将应能够查看内容的每个人添加到 Visitors 组，以及应能够管理自定义播放列表的所有人添加到 Members 组。 若要在用户第一次成为网站集管理员或 Owners 组的一部分时为自定义学习配置网站。

将 Office 365 应用的自定义学习添加到网站集。

## <a name="execute-powershell-configuration-script"></a>执行 PowerShell 配置脚本

包含一个 PowerShell 脚本，您需要执行该脚本来创建解决方案使用的三 `CustomLearningConfiguration.ps1` 个租户属性。 [](/sharepoint/dev/spfx/tenant-properties) 此外，该脚本在网站页面库中[](/sharepoint/dev/spfx/web-parts/single-part-app-pages)创建两个单部件应用程序页面，以在已知位置托管管理员和用户 Web 部件。

### <a name="disabling-telemetry-collection"></a>禁用遥测集合

此解决方案的一部分包括匿名遥测跟踪选择加入，默认情况下设置为"打开"。 如果要执行手动安装，并且要关闭遥测跟踪，请更改脚本以将 $optInTelemetry 变量设置为 `CustomlearningConfiguration.ps1` $false。

如果不执行手动安装，并且要关闭遥测跟踪，则包含单独的脚本，运行时 `TelemetryOptOut.ps1` 将禁用遥测跟踪。

## <a name="initialize-web-part-custom-configuration"></a>初始化 Web 部件自定义配置

成功运行 PowerShell 脚本后，导航到 `<YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx` 。 这将初始化 CustomConfig 列表项，该项设置自定义学习，供其首次使用。

配置现已完成，您可以使用自定义学习 for Office 365 继续操作。 有关详细信息，请参阅用户文档。
