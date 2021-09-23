---
author: pkrebs
ms.author: pkrebs
title: Learning ml 的手动设置路径
ms.date: 02/10/2019
description: Learning路径手动设置
ROBOTS: NOINDEX, NOFOLLOW
ms.service: sharepoint-online
manager: bpardi
ms.topic: article
ms.openlocfilehash: 89693e3020baa46f86b51b97c54240f12fec2d3a
ms.sourcegitcommit: a93cae8ea6e3c1141d7266d04131b69f2c2498cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/23/2021
ms.locfileid: "59485163"
---
# <a name="learning-pathways-manual-setup-for-multilingual"></a>Learning多语言的手动设置路径

Microsoft 365学习路径为需要以下方案之一支持的组织提供手动设置：

- 你的组织已建立一SharePoint Online 新式通信网站，专用于培训，并且你想要向该网站添加学习路径。 在此方案中，尚未在网站中设置学习路径 Web 部件。

- 您希望在组织的一个通信网站中安装多语言支持SharePoint路径。 该网站具有（或将具有）一种默认语言，该语言不是英语，并且是学习路径支持的语言之一。 以下是学习路径支持的语言：

- 英语
- 中文(简体)
- 法语
- 德语
- 意大利语（意大利）
- 日语（日本）
- 葡萄牙语（巴西）
- 俄语 (俄语) 
- 西班牙语

手动设置学习路径需要使用 Windows PowerShell 和 SharePoint Online 命令行管理程序的经验。 下面概述了手动设置学习路径的步骤： 

- 验证是否满足所有先决条件。
- 检查网站的默认语言设置。 如果确定，则继续手动安装。 如果您需要其他默认语言设置，则需要创建新网站。 
- 在租户应用程序目录中安装 customlearning.sppkg SharePoint文件。
- 设置/标识新式通信网站，以用作Microsoft 365学习路径主页。
- 执行 PowerShell 脚本，该脚本使用学习路径所依赖的项目配置租户。
- 导航到 CustomLearningAdmin.aspx 网站页面，以加载管理 Web 部件以初始化自定义内容配置。

## <a name="prerequisites"></a>必备条件
若要确保成功手动设置学习路径 Web 部件，必须满足以下先决条件。 

- 你必须已设置和配置租户范围的应用程序目录。 请参阅[设置租户Office 365](/sharepoint/dev/spfx/set-up-your-developer-tenant#create-app-catalog-site)并按照"创建应用程序目录"网站部分操作。 
- 如果租户范围的应用程序目录已预配，则需要访问具有将程序包上载到该帐户权限的帐户。 通常，此帐户具有SharePoint管理员角色。 
- 如果具有该角色的帐户不起作用，请转到 SharePoint 管理中心并查找应用程序目录网站集的网站集管理员，并作为网站集管理员之一登录，或者向网站集管理员添加失败的 SharePoint 管理员帐户。 
- 你还需要访问作为租户管理员SharePoint帐户。

## <a name="step-1---check-your-language-settings"></a>步骤 1 - 检查语言设置
作为手动安装过程的第一步，请检查网站语言设置。 以下是可能的选项：

### <a name="option-1---you-dont-want-multilingual-support"></a>选项 1 - 不需要多语言支持
如果您不希望为您的网站提供多语言支持，请确保其已关闭。
1.  From the SharePoint communication site， select **设置**  >  **Site information** View all site  >  **settings** Language  >  **settings**. 
2.  将 **"启用要翻译为多种语言的页面** 和新闻"开关设置为 **"关闭"。**
3.  单击“**保存**”。 
4.  继续执行步骤 2。

## <a name="option-2---you-want-multilingual-support-and-youre-ok-with-the-default-language"></a>选项 2 - 需要多语言支持，可以使用默认语言
一SharePoint通信网站具有默认语言。 默认语言确定您查看学习路径时使用的语言，包括学习路径管理页。 默认语言设置是在首次创建网站时设置的，以后无法更改。 在继续手动设置之前，请确保使用目标网站的默认语言确定。

1.  From the SharePoint communication site， select **设置**  >  **Site information** View all site  >  **settings** Language  >  **settings**. 
2.  将 **"启用要翻译为多种语言的页面** 和新闻"开关设置为 **"开"。**
    - If you're OK with the language that appears at the top of the list under **Language**， you can add additional languages， and then click **Save**. 继续执行步骤 2。
    - 如果您需要与为网站选择的语言不同的默认语言，则需要使用所需的语言SharePoint通信网站。 继续执行选项 3。 

## <a name="option-3---you-want-multilingual-support-but-want-a-different-default-language-for-the-site"></a>选项#3 - 您希望多语言支持，但需要网站的不同默认语言
使用此选项，可以创建一个SharePoint语言的新联机通信网站，然后设置该网站的语言设置。 
1.  若要创建新的通信SharePoint，请参阅在 SharePoint Online[中创建通信网站](https://support.microsoft.com/office/create-a-communication-site-in-sharepoint-online-7fb44b20-a72f-4d2c-9173-fc8f59ba50eb)。 创建网站时，请确保将语言设置为学习路径需要的默认语言。 
2. 从你创建的网站中 **，选择"设置**  >    >  **查看所有网站设置 语言**  >  **设置"。** 
2.  将 **"启用要翻译为多种语言的页面** 和新闻"开关设置为 **"开"。**
3. 如有必要，添加其他语言，然后单击"保存 **"。** 
4. 继续执行步骤 2。 

>![注意]如果需要将自定义内容从网站迁移到新创建的网站，请参阅本文档稍后的"迁移自定义内容"部分。 

## <a name="step-2---get-the-web-part-package-and-setup-script-from-github"></a>步骤 2 - 从网站获取 Web 部件包和GitHub
作为设置过程的一部分，你需要使用 Microsoft 365 Web 部件包和 PowerShell 安装脚本。

- 转到[存储库GitHub路径](https://github.com/pnp/custom-learning-office-365)。
- 单击 **"** 下载"将 Web 部件包和脚本保存到本地驱动器。 在此过程的稍后步骤中，你将使用脚本和 Web 部件包。

## <a name="step-2---upload-the-web-part-to-the-tenant-app-catalog"></a>步骤 2 - Upload Web 部件到租户应用程序目录
若要设置Microsoft 365路径，需要将 customlearning.sppkg 文件上载到租户范围的应用程序目录并部署它。 有关如何[将应用添加到应用程序目录的详细说明，请参阅](/sharepoint/use-app-catalog)使用应用程序目录为 SharePoint Online 环境提供自定义业务应用程序。

## <a name="step-3---provisionidentify-a-modern-communication-site"></a>步骤 3 - 预配/标识新式通信网站
确定现有SharePoint通信网站，或在 SharePoint Online 租户中预配新通信网站。 若要详细了解如何设置通信网站，请参阅在[SharePoint Online](https://support.office.com/article/create-a-communication-site-in-sharepoint-online-7fb44b20-a72f-4d2c-9173-fc8f59ba50eb)中创建通信网站并按照步骤创建通信网站。

## <a name="step-4---add-the-microsoft-365-learning-pathways-app-to-the-site"></a>步骤 4 - 将Microsoft 365学习路径应用添加到网站

1. 在"SharePoint"网站中，单击"系统"菜单，然后单击"**添加应用"。** 
2. 在 **"你的应用"** 下，单击"**来自你的组织**"，然后单击 **"Office 365"。** 

## <a name="step-5---set-permissions-for-the-site"></a>步骤 5 - 设置网站的权限
确保为网站设置了以下权限：
- **网站集管理员或 Owners** 组的一部分 - 初始化 CustomConfig 列表项所需的权限，可设置首次使用的学习路径。 
- **Members 组** - 管理学习路径（包括隐藏和显示内容以及管理自定义播放列表）所需的权限
- **Visitors 组** - 查看网站内容所需的权限。 

## <a name="step-6--execute-powershell-configuration-script"></a>步骤 6- 执行 PowerShell 配置脚本
包含一个 PowerShell 脚本，您需要执行该脚本来创建解决方案使用的三 `CustomLearningConfiguration.ps1` 个租户属性。 [](/sharepoint/dev/spfx/tenant-properties) 此外，该脚本在网站页面库中[](/sharepoint/dev/spfx/web-parts/single-part-app-pages)创建两个单部件应用程序页面，以在已知位置托管管理员和用户 Web 部件。

1. 如果尚未下载联机命令行管理程序SharePoint，立即下载。 请参阅[SharePoint Online 命令行管理程序下载](https://go.microsoft.com/fwlink/p/?LinkId=255251)。
2. 可能需要设置 PowerShell 执行策略来运行脚本。 有关详细信息，请参阅关于 [执行策略](/powershell/module/microsoft.powershell.core/about/about_execution_policies)。
3. 执行 `CustomLearningConfiguration.ps1` 脚本。 除了租户管理员凭据之外，脚本还将提示你输入租户名称和网站名称。 考虑以下网站 URL 示例， 是 `https://contoso.sharepoint.com/sites/O365CL` 租户 `contoso` 名称， `O365CL` 是网站名称。 

### <a name="disabling-telemetry-collection"></a>禁用遥测集合
此解决方案的一部分包括匿名遥测跟踪选择加入，默认情况下设置为"打开"。 如果要进行手动安装，并且要关闭遥测跟踪，请更改脚本以将 $optInTelemetry 变量设置为 $false `CustomlearningConfiguration.ps1` 并运行脚本。

## <a name="validate-provisioning-success-and-initialize-the-customconfig-list"></a>验证预配成功并初始化 CustomConfig 列表

成功运行 PowerShell 脚本后，导航到网站，初始化 **CustomConfig** 列表项，以设置首次使用的学习路径，并验证网站是否正常工作。

- 转到 `<YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx`。 打开 **CustomLearningAdmin.aspx** 会初始化 **CustomConfig** 列表项，以设置首次使用的学习路径。 应该会看到如下页面：

![管理应用page.png](media/cg-adminapppage.png)

## <a name="add-owners-to-site"></a>将所有者添加到网站
作为租户管理员，你不太可能是自定义网站的人，因此你需要为网站分配几个所有者。 所有者对网站拥有管理权限，因此可以修改网站页面和重新品牌。 他们还能够隐藏和显示通过学习路径 Web 部件提供的内容。 此外，他们能够生成自定义播放列表并将其分配给自定义子类别。  

1. 从 **"SharePoint设置"** 菜单中，单击"**网站权限"。**
2. 单击 **"高级权限设置"。**
3. 单击 **"所有者"的学习Office 365路径**。
4. 单击 **"**  >  **向此组添加新用户"，** 然后添加希望成为所有者的用户。 
5. 在"共享 ["消息中添加"浏览](custom_exploresite.md)网站"的链接，然后单击"共享 **"。**

## <a name="migrate-custom-content"></a>迁移自定义内容
按照上述步骤重新建立学习路径网站后，需要移动 **CustomPlaylists** 列表和 **CustomAssets 列表** 的内容。 如果自定义资产位于现有学习路径网站中，则还可以移动实际自定义页面（如果它们位于现有学习路径网站中，并且您打算将其删除）。 任务可能比较困难，因为对于 **CustomPlaylists** 列表中的所有项 **，CustomAssets** 列表中的列表项的 ID 将隐藏在每个播放列表列表项的 JSONData 字段中。 因此，仅将 **CustomPlaylists** 列表的内容从一个网站移动到另一个网站是不够的。 此外 **，CustomAssets** 列表包含列表项的 JSONData 字段中自定义资产页面的绝对 URL。 如果未移动资产，并且网站未重命名 (因此将绝对 URL 更改到资产的页面) ， **则 CustomAssets** 可以保留。 但需要手动更正条目。 鉴于这种类型的迁移的复杂性，我们建议你考虑招募我们的学习路径合作伙伴之一来帮助你进行此过渡。 

### <a name="next-steps"></a>后续步骤
- 请参阅 [自定义学习路径](custom_overview.md)。 
- 请参阅 [翻译网站页面](custom_translate_page_ml.md)。