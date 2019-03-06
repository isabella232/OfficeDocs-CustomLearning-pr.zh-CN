# <a name="manually-installing-and-configuring-custom-learning-for-office-365"></a>手动安装和配置适用于 Office 365 的自定义学习

Microsoft 自定义学习 Web 部件是使用[SharePoint 框架](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/sharepoint-framework-overview)版本1.7.1 生成的。

若要手动安装和配置 web 部件和网站集, 将需要完成以下步骤:

1. 验证是否已满足所有先决条件。
1. 在 Office 365 租户应用程序目录中安装 .sppkg 文件 customlearning。
1. 预配/确定要充当 Office 365 主网站的自定义学习的新式通信网站。
1. 执行 PowerShell 脚本, 该脚本将使用自定义学习所依赖的相应项目来配置租户。
1. 导航到 CustomLearningAdmin 网站页面, 以加载管理 web 部件以初始化自定义内容配置。

## <a name="prerequisites"></a>先决条件

您必须已设置和配置租户范围内的应用程序目录。 请参阅[设置您的 Office 365 租户](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/set-up-your-developer-tenant#create-app-catalog-site), 并遵循 "创建应用程序目录网站" 部分。 如果你的租户范围内的应用程序目录已设置, 你将需要访问有权将程序包上载到该帐户的帐户, 才能完成此安装过程。 通常情况下, 这是一个具有 SharePoint 管理员角色的帐户。 如果具有该角色的帐户不起作用, 请转到 SharePoint 管理中心并查找应用程序目录网站集的网站集管理员, 并以网站集管理员之一的身份登录, 或者添加 SharePoint 管理员帐户对网站集管理员失败。 您还需要具有对 SharePoint 租户管理员帐户的访问权限。

## <a name="upload-the-web-part-to-the-tenant-app-catalog"></a>将 web 部件上载到租户应用程序目录

若要设置针对 Office 365 的自定义学习, 请将 customlearning 文件上传到租户范围的应用程序目录并部署它。 有关如何将应用程序添加到应用程序目录的详细说明, 请参阅[使用应用程序目录为 SharePoint Online 环境提供自定义业务应用程序](https://docs.microsoft.com/en-us/sharepoint/use-app-catalog)。

## <a name="provisionidentify-modern-communication-site"></a>设置/确定新式通信网站

请在 sharepoint Online 租户中标识现有的 sharepoint 通信网站或设置新的 sharepoint 通信网站。 有关如何设置通信网站的详细信息, 请参阅[在 SharePoint Online 中创建通信网站](https://support.office.com/en-us/article/create-a-communication-site-in-sharepoint-online-7fb44b20-a72f-4d2c-9173-fc8f59ba50eb)和按照创建通信网站的步骤进行操作。

## <a name="set-permissions-for-the-site"></a>设置网站的权限

你将需要添加能够查看访问者组内容的所有人, 以及应能够将自定义播放列表管理到 Members 组中的每个人。 首次用户必须是网站集管理员或所有者组的一部分时, 才能将网站配置为自定义学习。

将适用于 Office 365 应用的自定义学习添加到网站集。

## <a name="execute-powershell-configuration-script"></a>执行 PowerShell 配置脚本

包含的 PowerShell `CustomLearningConfiguration.ps1`脚本将需要执行, 以创建解决方案使用的三个[租户属性](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/tenant-properties)。 此外, 该脚本将在网站页面库中创建两个[单独的部件应用程序页面](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/web-parts/single-part-app-pages), 以在已知位置承载管理员和用户 web 部件。

### <a name="disabling-telemetry-collection"></a>禁用遥测集合

此解决方案的一部分包括匿名遥测跟踪自愿加入, 默认情况下设置为 "开"。 如果要执行手动安装且要关闭遥测跟踪, 请更改`CustomlearningConfiguration.ps1`脚本以将 $optInTelemetry 变量设置为 $false。

如果您未执行手动安装且要关闭遥测跟踪, 则在运行将禁用遥测跟踪时`TelemetryOptOut.ps1` , 将会包含单独的脚本。

## <a name="initialize-web-part-custom-configuration"></a>初始化 web 部件自定义配置

成功运行 PowerShell 脚本后, 导航到`<YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx`。 这将初始化为其首次使用设置自定义学习的 CustomConfig 列表项。

现在配置已完成, 您可以使用适用于 Office 365 的自定义学习向前移动。 有关详细信息, 请参阅用户文档。