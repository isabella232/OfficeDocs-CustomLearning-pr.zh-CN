---
author: pkrebs
ms.author: pkrebs
title: 学习路径手动设置
ms.date: 02/10/2019
description: 学习路径手动设置
ROBOTS: NOINDEX, NOFOLLOW
ms.openlocfilehash: c524ebae73cb928a8e77567d4ea2c5e8d5032ccd
ms.sourcegitcommit: f355885fb93d66abf61df535fa704ccdb8df9b64
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/05/2020
ms.locfileid: "45038972"
---
# <a name="learning-pathways-manual-setup"></a>学习路径手动设置

Microsoft 365 学习通道为需要支持下列方案之一的组织提供手动设置：

- 您的组织具有专用于培训的 SharePoint Online 新式通信网站，您想要添加到该网站的学习途径。 在这种情况下，尚未在网站上设置 "学习路径" web 部件。

- 您想要在某个组织的 SharePoint 通信网站中安装多语言支持的学习路径。 该网站具有或将具有非英语的默认语言，并且是学习路径支持的语言之一。 以下是学习途径支持的语言：

- English
- 中文(简体)
- 法语
- 德语
- 意大利语（意大利）
- 日语（日本）
- 葡萄牙语（巴西）
- 俄语（俄语）
- 西班牙语

手动设置学习路径需要使用 Windows PowerShell 和 SharePoint Online 命令行管理程序。 下面概述了手动设置学习路径的步骤： 

- 验证是否已满足所有先决条件。
- 检查网站的默认语言设置。 如果确定，请继续手动安装。 如果需要不同的默认语言设置，则需要创建新网站。 
- 在您的 SharePoint 租户应用程序目录中安装 customlearning 文件。
- 设置/确定要充当 Microsoft 365 学习路径主网站的新式通信网站。
- 执行 PowerShell 脚本，将您的租户配置为学习路径所依赖的项目。
- 导航到 CustomLearningAdmin 网站页面，以加载管理 web 部件以初始化自定义内容配置。

## <a name="prerequisites"></a>先决条件
为确保成功手动设置学习路径 web 部件，必须满足以下先决条件。 

- 您必须已设置和配置租户范围内的应用程序目录。 请参阅[设置 Office 365 租户](https://docs.microsoft.com/sharepoint/dev/spfx/set-up-your-developer-tenant#create-app-catalog-site)和跟踪 "创建应用程序目录" 网站部分。 
- 如果你的租户范围内的应用程序目录已预配，你将需要访问有权将程序包上载到其中的帐户。 通常，此帐户具有 SharePoint 管理员角色。 
- 如果具有该角色的帐户不起作用，请转到 SharePoint 管理中心，并查找应用程序目录网站集的网站集管理员，然后以网站集管理员身份登录，或添加 SharePoint 管理员帐户，以使网站集管理员失败。 
- 你还需要具有对 SharePoint 租户管理员帐户的访问权限。

## <a name="step-1---check-your-language-settings"></a>第1步-检查您的语言设置
作为手动安装过程的第一步，请检查您的网站语言设置。 以下是可能的选项：

### <a name="option-1---you-dont-want-multilingual-support"></a>选项 1-不需要多语言支持
如果您不希望对网站进行多语言支持，请确保已将其关闭。
1.  在 SharePoint 通信网站中，选择 "**设置**  >  **网站信息**"  >  **查看 "所有网站设置**  >  **语言设置**"。 
2.  将 "**允许将页面和新闻转换为多种语言**" 开关设置为 "**关闭**"。
3.  单击“保存”****。 
4.  继续执行步骤2。

## <a name="option-2---you-want-multilingual-support-and-youre-ok-with-the-default-language"></a>选项 2-您需要多语言支持，并且您可以使用默认语言
SharePoint 通信网站具有默认语言。 默认语言确定查看学习路径的语言，包括 "学习路径管理" 页面。 默认语言设置是在首次创建网站时设置的，不能在此后更改。 在使用手动设置 Continueing 之前，请确保您是目标网站的默认语言的 "正常"。

1.  在 SharePoint 通信网站中，选择 "**设置**  >  **网站信息**"  >  **查看 "所有网站设置**  >  **语言设置**"。 
2.  将 "**启用要转换为多种语言的页面和新闻**" 设置为 **"打开"**。
    - 如果您使用 "**语言**" 下列表顶部显示的语言，则可以添加其他语言，然后单击 "**保存**"。 继续执行步骤2。
    - 如果您需要与为网站选择的默认语言不同的默认语言，则需要使用所需的语言创建新的 SharePoint 通信网站。 继续选择 "3"。 

## <a name="option-3---you-want-multilingual-support-but-want-a-different-default-language-for-the-site"></a>选项 #3-您需要多语言支持，但需要网站的不同默认语言
使用此选项，您可以使用所需的默认语言创建新的 SharePoint Online 通信网站，然后设置该网站的语言设置。 
1.  若要创建新的 SharePoint 通信网站，请参阅[在 SharePoint Online 中创建通信网站](https://support.microsoft.com/office/create-a-communication-site-in-sharepoint-online-7fb44b20-a72f-4d2c-9173-fc8f59ba50eb)。 创建网站时，请务必将语言设置为学习路径所需的默认语言。 
2. 在您创建的网站中，选择 "**设置**  >  **网站信息**"  >  **查看 "所有网站设置**  >  **语言设置**"。 
2.  将 "**启用要转换为多种语言的页面和新闻**" 设置为 **"打开"**。
3. 如有必要，添加其他语言，然后单击 "**保存**"。 
4. 继续执行步骤2。 

>!便笺如果需要将自定义内容从网站迁移到新创建的网站，请参阅本文档后面的 "迁移自定义内容" 一节。 

## <a name="step-2---get-the-web-part-package-and-setup-script-from-github"></a>第2步-获取 GitHub 中的 web 部件包和安装脚本
作为安装过程的一部分，你将需要 Microsoft 365 学习路径 Web 部件包和 PowerShell 安装脚本。

- 转到 "[学习路径 GitHub 存储库](https://github.com/pnp/custom-learning-office-365)"。
- 单击 "**下载**" 将 web 部件包和脚本保存到本地驱动器。 您将在此过程的后续步骤中使用脚本和 web 部件包。

## <a name="step-2---upload-the-web-part-to-the-tenant-app-catalog"></a>步骤 2-将 web 部件上传到租户应用程序目录
若要设置 Microsoft 365 学习路径，请将 customlearning 文件上传到租户范围的应用程序目录并部署它。 有关如何将应用程序添加到应用程序目录的详细说明，请参阅[使用应用程序目录为 SharePoint Online 环境提供自定义业务应用程序](https://docs.microsoft.com/sharepoint/use-app-catalog)。

## <a name="step-3---provisionidentify-a-modern-communication-site"></a>第3步-设置/确定新式通信网站
请在 SharePoint Online 租户中标识现有的 SharePoint 通信网站或设置新的 SharePoint 通信网站。 有关如何设置通信网站的详细信息，请参阅[在 SharePoint Online 中创建通信网站](https://support.office.com/en-us/article/create-a-communication-site-in-sharepoint-online-7fb44b20-a72f-4d2c-9173-fc8f59ba50eb)和按照创建通信网站的步骤进行操作。

## <a name="step-4---add-the-microsoft-365-learning-pathways-app-to-the-site"></a>步骤 4-向网站添加 Microsoft 365 学习路径应用程序

1. 在 SharePoint 网站中，单击 "系统" 菜单，然后单击 "**添加应用程序**"。 
2. 在**您的应用程序**下，单击**您的组织**，然后单击 "**了解 Office 365 的路径**"。 

## <a name="step-5---set-permissions-for-the-site"></a>步骤 5-设置网站的权限
确保为网站设置了以下权限：
- **网站集管理员或所有者组的一部分**-初始化 CustomConfig 列表项以设置其首次使用的学习路径所需的权限。 
- **Members 组**-管理学习路径所需的权限，包括隐藏和显示内容以及管理自定义播放列表
- **访问者组**-查看网站内容所需的权限。 

## <a name="step-6--execute-powershell-configuration-script"></a>步骤 6-执行 PowerShell 配置脚本
包含的 PowerShell 脚本 `CustomLearningConfiguration.ps1` 将需要执行，以创建解决方案使用的三个[租户属性](https://docs.microsoft.com/sharepoint/dev/spfx/tenant-properties)。 此外，该脚本将在网站页面库中创建两个[单独的部件应用程序页面](https://docs.microsoft.com/sharepoint/dev/spfx/web-parts/single-part-app-pages)，以在已知位置承载管理员和用户 web 部件。

1. 如果还未下载 SharePoint Online 命令行管理程序，请立即下载。 请参阅[SharePoint Online 命令行管理程序下载](https://go.microsoft.com/fwlink/p/?LinkId=255251)。
2. 您可能需要设置 PowerShell 执行策略以运行脚本。 有关详细信息，请参阅[关于执行策略](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)。
3. 执行 `CustomLearningConfiguration.ps1` 脚本。 除了租户管理员凭据之外，该脚本还会提示你输入租户名称和站点名称。 考虑网站 URL 的以下示例， `https://contoso.sharepoint.com/sites/O365CL` `contoso` 是租户名称，也 `O365CL` 是网站名称。 

### <a name="disabling-telemetry-collection"></a>禁用遥测集合
此解决方案的一部分包括匿名遥测跟踪自愿加入，默认情况下设置为 "开"。 如果要执行手动安装且要关闭遥测跟踪，请更改 `CustomlearningConfiguration.ps1` 脚本以将 $optInTelemetry 变量设置为 $false 并运行脚本。

## <a name="validate-provisioning-success-and-initialize-the-customconfig-list"></a>验证设置是否成功并初始化 CustomConfig 列表

在成功运行 PowerShell 脚本之后，您将导航到该网站，初始化**CustomConfig**列表项，该列表项将设置第一次使用的学习路径，并验证网站是否正常工作。

- 转到 `<YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx`。 打开**CustomLearningAdmin**可初始化**CustomConfig**列表项，该列表项设置首次使用的学习路径。 您应该会看到如下所示的页面：

![cg-adminapppage.png](media/cg-adminapppage.png)

## <a name="add-owners-to-site"></a>将所有者添加到网站
作为租户管理员，您不太可能是自定义网站的人员，因此您需要向网站分配一些所有者。 所有者具有对网站的管理权限，以便他们可以修改网站页面并 rebrand 网站。 他们还能够隐藏和显示通过 "学习路径" Web 部件传递的内容。 此外，他们还能够构建自定义播放列表并将其分配给自定义子类别。  

1. 从 "SharePoint**设置**" 菜单中，单击 "**网站权限**"。
2. 单击 "**高级权限设置**"。
3. 单击 " **Office 365 所有者的学习路径**"。
4. 单击 "**新建**向  >  **此组添加用户**"，然后添加您希望成为所有者的人员。 
5. 添加链接以在共享邮件中[浏览网站](https://docs.microsoft.com/Office365/CustomLearning/custom_explore)，然后单击 "**共享**"。

## <a name="migrate-custom-content"></a>迁移自定义内容
在您按照上述步骤重新建立学习路径网站后，您需要移动**CustomPlaylists**列表和**CustomAssets**列表的内容。 此外，您还可以在现有的学习路径网站中，移动构成自定义资产的实际自定义页面，并且您的意图是将其删除。 任务可能很困难，因为对于**CustomPlaylists**列表中的所有项， **CustomAssets**列表中的列表项的 ID 将隐藏在每个播放列表项的 JSONData 字段中。 因此，只需将**CustomPlaylists**列表中的内容从一个网站移到另一个网站即可。 此外， **CustomAssets**列表包含列表项的 JSONData 字段中自定义资产页面的绝对 URL。 如果资产未移动，并且网站未重命名（从而将绝对 URL 更改为资产页面），则**CustomAssets**可以保留。 但您需要手动更正这些条目。 考虑到这种类型的迁移的复杂性，我们建议您考虑登记我们的一个学习路径合作伙伴，以帮助您进行此转换。 

### <a name="next-steps"></a>后续步骤
- 请参阅[自定义学习路径](custom_overview.md)。 
- 请参阅[翻译网站页面](custom_translate_page_ml.md)。

