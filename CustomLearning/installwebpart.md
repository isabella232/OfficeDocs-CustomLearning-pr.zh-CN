# <a name="installing-the-custom-learning-solution-webpart"></a>安装自定义学习解决方案 web 部件

## <a name="prerequisites-for-a-tenant-wide-installation"></a>租户范围内安装先决条件

- 为您的整个租户安装自定义学习 web 部件需要具有 Office 365 管理权限。 如果您没有这些权限，您可以使用 Office 365 管理员或安装的单个网站集的 web 部件。
- 您或您的 Office 365 管理员必须安装和配置租户范围[应用程序目录](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/set-up-your-developer-tenant)或[网站集应用程序目录](https://docs.microsoft.com/en-us/sharepoint/dev/general-development/site-collection-app-catalog)，以接收 web 部件。]
- 我们仅支持 SharePoint Online。Web 部件不支持任何版本的本地 SharePoint 安装。

## <a name="add-the-custom-learning-webpart-to-your-tenant"></a>将自定义学习 web 部件添加到您的租户 

1. 下载自定义学习 web 部件并将其保存到本地驱动器。 此文件被命名为"ms 自定义 learning.sppkg"。 不要更改的名称或文件的后缀。 
2. 导航到[Office 365 管理门户](https://admin.microsoft.com/AdminPortal/Home#/homepage)租户
3. 左侧导航栏上选择管理中心，SharePoint。这将打开新选项卡中，选择在 SharePoint 管理中心的应用程序、 应用程序目录、 SharePoint 相关应用程序中 
4. 选择上载 web 部件，并选择"ms 自定义 learning.sppkg"文件下载
5. 为此租户范围内安装检查"使可用于所有此解决方案位于组织中。"旁边的框  

![部署解决方案](media/trustapp_sm.png)


## <a name="add-the-customer-learning-webpart-to-a-sharepoint-online-page"></a>将客户学习 web 部件添加到 SharePoint Online 网页

自定义学习安装在您的租户后您可以向 SharePoint 页面添加 Web 部件。执行操作时，突然 Office 365 培训可供您。 

1. 在整个宽度的列布局中添加自定义学习 web 部件：

![SharePoint 页面布局](media/clo365fullcolumnwidth.png)

2. 在 SharePoint 页中，选择添加一节，然后选择完整宽度的列。 您将看到以下提示：

![AddWebpart](media/clo365addfullwidthwebpart.png)

3. 选择 Microsoft Learning。 您现在应该看到以下： 

![学习 web 部件的自定义](media/clo365addwebpart.png)

 您现在可以单击拼贴来分析解决方案中包含的默认内容。  

## <a name="next-steps"></a>后续步骤
- 浏览包括 web 部件中的[默认内容](webpartcontent.md)。
- [自定义](customization.md)您的组织的培训体验。
- 培训解决方案的[驱动器应用](driveadoption.md)。

