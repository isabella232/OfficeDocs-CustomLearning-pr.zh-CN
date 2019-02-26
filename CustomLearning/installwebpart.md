---
author: karuanag
ms.author: karuanag
title: 安装自定义学习解决方案 web 部件
ms.date: 02/10/2019
description: 自定义学习解决方案 web 部件的安装说明
ms.openlocfilehash: 53229e5b1b8175b06d888091963d1a9f2f0bd361
ms.sourcegitcommit: e10085e60ca3f38029fde229fb093e6bc4a34203
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/25/2019
ms.locfileid: "29989683"
---
# <a name="installing-the-custom-learning-solution-webpart"></a>安装自定义学习解决方案 web 部件

## <a name="prerequisites-for-a-tenant-wide-installation"></a>租户范围安装的先决条件

- 若要为你的整个租户安装自定义的学习 web 部件, 你需要具有 Office 365 管理权限。 如果您没有这些权限, 则可以与 Office 365 管理员合作, 也可以为单个网站集安装 web 部件。
- 您或您的 Office 365 管理员必须已安装并配置了租户范围的[应用程序目录](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/set-up-your-developer-tenant)或[网站集应用程序目录](https://docs.microsoft.com/en-us/sharepoint/dev/general-development/site-collection-app-catalog), 才能接收 web 部件。]
- 我们仅支持 SharePoint Online。web 部件不支持在本地的任何 SharePoint 版本上安装。

## <a name="add-the-custom-learning-webpart-to-your-tenant"></a>将自定义学习 web 部件添加到租户 

1. 下载自定义学习 web 部件并将其保存到本地驱动器。 此文件名为 "ms-自定义 .sppkg"。 不要更改文件的名称或后缀。 
2. 导航到适用于租户的[Office 365 管理门户](https://admin.microsoft.com/AdminPortal/Home#/homepage)
3. 从左侧导航中选择 "管理中心"、"SharePoint"。这将在新选项卡中打开。, 在 SharePoint 管理中心中选择 "应用程序"、"应用程序目录" 和 "SharePoint 相关应用程序" 
4. 选择 "上载 web 部件", 然后选择您下载的 "ms-自定义 .sppkg" 文件
5. 对于此租户范围的安装, 请选中 "使此解决方案可供组织中的所有公司使用" 旁边的复选框。  
 
> [!NOTE]
> 安装 webpart 后, 即可在 SharePoint Online 的 web 部件库中找到它。 **在库中, web 部件名为 "Microsoft 学习"**

![部署解决方案](media/trustapp_sm.png)


## <a name="add-the-microsoft-learning-webpart-to-a-sharepoint-online-page"></a>将 Microsoft 学习 web 部件添加到 SharePoint Online 页面

在租户中安装自定义学习后, 可以将 Web 部件添加到 SharePoint 页面。当你执行 Office 365 和 Windows 10 培训时, 你的网站可供你使用。

1. 在全宽列布局中添加自定义学习 web 部件:

![SharePoint 页面布局](media/clo365fullcolumnwidth.png)

2. 在 SharePoint 页面中, 选择 "添加内容", 然后选择 "全宽列"。 您将看到以下提示:

![AddWebpart](media/clo365addfullwidthwebpart.png)

3. 选择 "Microsoft 学习"。 您现在应该会看到以下内容: 

![自定义学习 web 部件](media/clo365addwebpart.png)

 您现在可以单击磁贴来浏览解决方案中包含的默认内容。  

### <a name="next-steps"></a>后续步骤
- 浏览 web 部件中包含的[默认内容](webpartcontent.md)。
- 为你的组织[自定义](customization.md)培训体验。
- [促进](driveadoption.md)培训解决方案的采用。

