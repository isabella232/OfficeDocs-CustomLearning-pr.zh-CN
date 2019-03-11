---
author: pkrebs
ms.author: pkrebs
title: 独立 web 部件设置
ms.date: 02/10/2019
description: 适用于 Office 365 的自定义学习手动 web 部件设置
ms.openlocfilehash: f5d94d673f491d5b5778ef73d518914dbd4cdbb9
ms.sourcegitcommit: e0adc8963419a4dd5c4d9bcc9f4f2cc1fbe291d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/10/2019
ms.locfileid: "30523056"
---
# <a name="stand-alone-web-part-setup"></a>独立 web 部件设置

自定义学习为已建立 SharePoint Online 新式通信网站的组织提供手动、独立的 web 部件设置, 或者只需设置自己的自定义学习 web 部件通信网站。 请注意, 手动安装需要使用 Windows PowerShell 和 SharePoint Online 命令行管理程序。 手动设置自定义学习 Web 部件的步骤如下所示:

- 验证是否已满足所有先决条件。
- 在 Office 365 租户应用程序目录中安装 .sppkg 文件 customlearning。
- 预配/确定要充当 Office 365 主网站的自定义学习的新式通信网站。
- 执行 PowerShell 脚本, 该脚本将使用自定义学习所依赖的相应项目来配置租户。
- 导航到 CustomLearningAdmin 网站页面, 以加载管理 web 部件以初始化自定义内容配置。

> [!NOTE]
> 如果你正在寻找一种快速、简便的方法来设置自定义学习, 请参阅[设置自定义学习](installsitepackage.md)。

## <a name="prerequisites"></a>先决条件
为了确保成功手动设置自定义的学习 web 部件, 必须满足以下先决条件。 

- 您必须已设置和配置租户范围内的应用程序目录。 请参阅[设置您的 Office 365 租户](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/set-up-your-developer-tenant#create-app-catalog-site), 并遵循 "创建应用程序目录网站" 部分。 
- 如果你的租户范围内的应用程序目录已设置, 你将需要访问有权将程序包上载到该帐户的帐户, 才能完成此安装过程。 通常情况下, 这是一个具有 SharePoint 管理员角色的帐户。 
- 如果具有该角色的帐户不起作用, 请转到 SharePoint 管理中心并查找应用程序目录网站集的网站集管理员, 并以网站集管理员之一的身份登录, 或者添加 SharePoint 管理员帐户对网站集管理员失败。 
- 您还需要具有对 SharePoint 租户管理员帐户的访问权限。

## <a name="step-1---get-the-web-part-package-and-setup-script-from-github"></a>步骤 1-从 GitHub 获取 web 部件包和安装脚本
在安装过程中, 你将需要自定义学习 Web 部件包和 PowerShell 安装脚本。

- 转到[自定义学习 GitHub 存储库](https://github.com/pnp/custom-learning-office-365)。
- 单击 "**下载**" 将 web 部件包和脚本保存到本地驱动器。 您将在此过程的后续步骤中使用脚本和 web 部件包。

## <a name="step-2---upload-the-web-part-to-the-tenant-app-catalog"></a>步骤 2-将 web 部件上传到租户应用程序目录
若要设置针对 Office 365 的自定义学习, 请将 customlearning 文件上传到租户范围的应用程序目录并部署它。 有关如何将应用程序添加到应用程序目录的详细说明, 请参阅[使用应用程序目录为 SharePoint Online 环境提供自定义业务应用程序](https://docs.microsoft.com/en-us/sharepoint/use-app-catalog)。

## <a name="step-3---provisionidentify-a-modern-communication-site"></a>第3步-设置/确定新式通信网站
请在 sharepoint Online 租户中标识现有的 sharepoint 通信网站或设置新的 sharepoint 通信网站。 有关如何设置通信网站的详细信息, 请参阅[在 SharePoint Online 中创建通信网站](https://support.office.com/en-us/article/create-a-communication-site-in-sharepoint-online-7fb44b20-a72f-4d2c-9173-fc8f59ba50eb)和按照创建通信网站的步骤进行操作。

## <a name="step-4---set-permissions-for-the-site"></a>步骤 4-设置网站的权限
确保为网站设置了以下权限:
- **网站集管理员或所有者组的一部分**-初始化 CustomConfig 列表项以设置首次使用的自定义学习所需的权限。 
- **Members 组**-管理自定义学习所需的 permissons, 包括隐藏和显示内容以及管理自定义播放列表
- **访问者组**-查看网站内容所需的权限。 

## <a name="step-5--execute-powershell-configuration-script"></a>第5步-执行 PowerShell 配置脚本
包含的 PowerShell `CustomLearningConfiguration.ps1`脚本将需要执行, 以创建解决方案使用的三个[租户属性](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/tenant-properties)。 此外, 该脚本将在网站页面库中创建两个[单独的部件应用程序页面](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/web-parts/single-part-app-pages), 以在已知位置承载管理员和用户 web 部件。

### <a name="disabling-telemetry-collection"></a>禁用遥测集合
此解决方案的一部分包括匿名遥测跟踪自愿加入, 默认情况下设置为 "开"。 如果要执行手动安装且要关闭遥测跟踪, 请更改`CustomlearningConfiguration.ps1`脚本以将 $optInTelemetry 变量设置为 $false。

如果您未执行手动安装且要关闭遥测跟踪, 则在运行将禁用遥测跟踪时`TelemetryOptOut.ps1` , 将会包含单独的脚本。

## <a name="validate-provisioning-success-and-initialize-the-customconfig-list"></a>验证设置是否成功并初始化 CustomConfig 列表

在成功运行 PowerShell 脚本之后, 您将导航到该网站, 初始化**CustomConfig**列表项, 该列表项会为首次使用设置自定义学习, 并验证网站是否正常工作。

1. 转到 `<YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx`。 打开**CustomLearningAdmin**可初始化**CustomConfig**列表项, 该列表项设置自定义学习以供首次使用。 您应该会看到如下所示的页面:

![cg-adminapppage](media/cg-adminapppage.png)

## <a name="add-owners-to-site"></a>将所有者添加到网站
作为租户管理员, 您不太可能是自定义网站的人员, 因此您需要向网站分配一些所有者。 所有者具有对网站的管理权限, 以便他们可以修改网站页面并 rebrand 网站。 他们还能够隐藏和显示通过自定义学习 Web 部件传递的内容。 此外, 他们还能够构建自定义播放列表并将其分配给自定义子类别。  

1. 从 "SharePoint**设置**" 菜单中, 单击 "**网站权限**"。
2. 单击 "**高级权限设置**"。
3. 单击 "**自定义学习 for Office 365 所有者**"。
4. 单击 "**新建** > 向**此组添加用户**", 然后添加您希望成为所有者的人员。 
5. 添加链接以在共享邮件中[浏览网站](https://docs.microsoft.com/en-us/Office365/CustomLearning/custom_explore), 然后单击 "**共享**"。

### <a name="next-steps"></a>后续步骤
- 为你的组织[自定义](custom_overview.md)培训体验。

