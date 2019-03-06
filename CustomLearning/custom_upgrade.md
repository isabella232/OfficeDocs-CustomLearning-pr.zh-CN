---
author: pkrebs
ms.author: pkrebs
title: 自定义学习升级
ms.date: 02/10/2019
description: 适用于 Office 365 的自定义学习手动 web 部件设置
ms.openlocfilehash: f9729c922b374cc6b775737fa7c7c76a4719534c
ms.sourcegitcommit: b6617bbbaee0784d6216e96052c2469f97cf51e9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2019
ms.locfileid: "30411892"
---
# <a name="manual-upgrade-for-custom-learning"></a>自定义学习的手动升级

适用于 Office 365 的自定义学习为参与早期试点的组织提供了手动升级过程。 在升级过程中, 组织可以通过将新的增强型自定义学习 web 部件添加到其 SharePoint 应用程序目录中, 然后运行 PowerShell 脚本, 来继续使用其当前的自定义学习网站并进行升级。 下面提供了升级过程的概述: 

- 验证负责上载新 web 部件和运行 Powershell 脚本的人员是否具有所需的权限
- 将 web 部件 .sppkg 文件上传到 Office 365 租户应用程序目录 customlearning
- 执行 PowerShell 脚本, 将您的租户配置为自定义学习所需的相应项目
- 导航到自定义学习网站中的 "CustomLearningAdmin" 页面, 以初始化自定义 Ccontent 配置。

## <a name="prerequisites"></a>先决条件
为了确保成功升级自定义学习, 必须满足以下先决条件。 

- 您必须已设置租户范围内的应用程序目录。 如果您没有租户应用程序目录, 请参阅[设置 Office 365 租户](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/set-up-your-developer-tenant#create-app-catalog-site)和遵循创建应用程序目录网站部分。 
- 如果已设置租户范围内的应用程序目录, 则需要访问有权将程序包上载到的帐户。 通常情况下, 这是一个具有 SharePoint 管理员角色的帐户。 
- 如果具有 SharePoint 管理员角色的帐户不起作用: 转到 "sharepoint 管理中心", 选择 "应用程序目录", 单击 "所有者", 然后以网站集管理员之一身份登录, 或添加对网站失败的 SharePoint 管理员帐户。集合管理员列表。 

## <a name="step-1---get-the-web-part-package-and-setup-script-from-github"></a>步骤 1-从 GitHub 获取 web 部件包和安装脚本
在安装过程中, 你将需要自定义学习 Web 部件包和 PowerShell 安装脚本。

1. 转到[自定义学习 GitHub 存储库](https://github.com/pnp/custom-learning-office-365)。
2. 单击 "**复制" 或 "下载**", 然后**下载 ZIP**。   
3. 将**ZIP**文件保存到本地驱动器上的某个位置。
4. 解压缩本地驱动器上的**ZIP**文件。

## <a name="step-2---upload-the-web-part-to-the-tenant-app-catalog"></a>步骤 2-将 web 部件上传到租户应用程序目录
若要设置针对 Office 365 的自定义学习, 请将 customlearning 文件上传到租户范围的应用程序目录并部署它。 有关如何将应用程序添加到应用程序目录的详细说明, 请参阅[使用应用程序目录为 SharePoint Online 环境提供自定义业务应用程序](https://docs.microsoft.com/en-us/sharepoint/use-app-catalog)。

1. 在 Office 365 中, 单击 "**管理员**"。
2. 在 "**管理中心**" 下, 单击 " **SharePoint**"。
3. 单击 "**应用** > **应用程序目录** > **分发 SharePoint 相关应用**程序"。
4. 单击 "**上载** > **选择文件**"。
5. 在保存 ZIP 文件的文件夹中, 选择 " **web 部件**" 文件夹, 然后选择 " **customlearning** " ".sppkg"。
6. 单击“部署”****。

## <a name="step-5--execute-powershell-configuration-script"></a>第5步-执行 PowerShell 配置脚本
来自 GitHub 的`CustomLearningConfiguration.ps1` ZIP 下载中包含一个 PowerShell 脚本。 您需要执行脚本以创建解决方案使用的三个[租户属性](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/tenant-properties)。 此外, 该脚本将在网站页面库中创建两个[单独的部件应用程序页面](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/web-parts/single-part-app-pages), 以在已知位置承载管理员和用户 web 部件。 这些应用程序页面为:

- CustomAdministration
- CustomViewer

### <a name="to-run-the-powershell-script"></a>运行 Powershell 脚本
- 使用 PowerShell, 从 GitHub `CustomLearningConfiguration.ps1` ZIP 执行 web 部件文件夹中的脚本。 如果成功, 你将在命令窗口中看到三个键/值对和**自定义的学习管理员。 ...**

### <a name="disabling-telemetry-collection"></a>禁用遥测集合
自定义学习包括匿名遥测跟踪自愿加入, 默认情况下设置为 "开"。 如果要关闭遥测跟踪, 请更改`CustomlearningConfiguration.ps1`脚本以将`$optInTelemetry`变量设置为。 `$false`

## <a name="step-6---initialize-web-part-custom-configuration"></a>步骤 6-初始化 web 部件自定义配置
成功运行 PowerShell 脚本后, 导航到`<YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx`。 打开**CustomLearningAdmin**可初始化**CustomConfig**列表项, 该列表项设置自定义学习以供首次使用。 您应该会看到如下所示的页面:

![cg-adminapppage](media/cg-adminapppage.png)

## <a name="add-owners-to-site"></a>将所有者添加到网站
作为租户管理员, 您不太可能是自定义网站的人员, 因此您需要向网站分配一些所有者。 所有者具有对网站的管理权限, 以便他们可以修改网站页面并 rebrand 网站。 他们还能够隐藏和显示通过自定义学习 Web 部件传递的内容。 他们还能够构建自定义播放列表并将其分配给自定义子类别。  

1. 从 "SharePoint**设置**" 菜单中, 单击 "**网站权限**"。
2. 单击 "**高级权限设置**"。
3. 单击 "**自定义学习 for Office 365 所有者**"。
4. 单击 "**新建** > 向**此组添加用户**", 添加您希望成为所有者的人员, 然后单击 "**共享**"。

升级现已完成。 若要详细了解如何为您的环境量身定制自定义的学习网站和 web 部件, 请参阅[自定义培训体验](custom_overview.md)。

## <a name="upgrade-instructions-for-site-owners"></a>网站所有者的升级说明
针对 office 365 的自定义学习已引入了对 web 部件的各种增强功能。 "[自定义学习体验](custom_overview.md)" 一节中详细介绍了如何使用 web 部件。 目前, 网站所有者应执行以下操作:  

- 验证 "Office 365 的自定义学习" Web 部件是否可用。 
- 将页面上的现有 web 部件替换为新 web 部件
- 替换指向旧 web 部件的任何链接

### <a name="verify-the-custom-learning-for-office-365-web-part-is-available"></a>验证 "Office 365 自定义学习" web 部件是否可用
1.  在自定义学习网站中, 单击 "**设置**", 然后单击 "***添加页面**"。
2.  单击页面**+** 上的图标以添加 web 部件, 然后选择 "**适用于 Office 365 的自定义学习**" web 部件。 此时, 页面看起来应类似于下图:

[cg-adminapppage](media/cg-adminapppage.png)
 
### <a name="replace-the-old-web-part-with-the-new-web-part"></a>将旧 web 部件替换为新的 web 部件
在替换自定义学习 web 部件或对网站进行更改之前, 我们建议您阅读[自定义学习体验](custom_overview.md)文档, 因为它说明了如何使用新的 web 部件。 

若要升级自定义学习网站, 请将 web 部件的现有实例替换为新的 web 部件。 虽然我们无法确定添加 web 部件的位置, 但以前的试验指南是将 web 部件添加到以下页面, 因此, 请查看以下页面上的 "替换 web 部件":

- Get-started-with-Office-365
- Get-started-with-Microsoft-Teams
- Get-started-with-OneDrive
- Get-started-with-SharePoint

### <a name="replace-existing-links-to-the-web-part"></a>替换指向 web 部件的现有链接
通过对新 web 部件的增强功能, 链接到播放列表的方法也发生了变化。 作为升级的一部分, 您应替换任何指向 web 部件的链接, 包括菜单项和主页上的链接。 在替换自定义学习 web 部件或对网站进行更改之前, 我们建议您阅读[自定义学习体验](custom_overview.md)文档, 因为它说明了如何使用新的 web 部件。 

## <a name="recreate-existing-playlists"></a>重新创建现有播放列表 
为了确保播放列表正常工作, 需要重新创建使用该 web 部件的早期版本创建的任何播放列表。 在删除播放列表之前, 请列出自定义播放列表和关联的资产, 以便您可以使用新的自定义学习 Web 部件轻松地重新创建它们。 创建一个播放列表副本, 然后将其删除。 您可以使用 JSONData 域在删除前复制播放列表的内容。 这将便于以后创建。


•在自定义学习网站中, 单击 "设置" > "网站内容"。 •选择一个播放列表, 选择省略号, 选择 "编辑", 然后复制 "JSONData" 字段的内容并保存在 "记事本" 或单独的文档中, 以供以后参考。 选择 "取消"。
•选择该播放列表, 选择省略号, 然后选择 "删除"。
•现在您可以使用新的 Web 部件重新创建播放列表。
有关使用新的自定义学习 for Office 365 Web 部件的说明, https://docs.microsoft.com/en-us/office365/customlearning/custom_overview请参阅。

## <a name="step-8---chan"></a>步骤 8-Chan

### <a name="next-steps"></a>后续步骤
- 为你的组织[自定义](custom_overview.md)培训体验。

