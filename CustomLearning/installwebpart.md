# <a name="installing-the-custom-learning-solution-webpart"></a><span data-ttu-id="dc9c5-101">安装自定义学习解决方案 web 部件</span><span class="sxs-lookup"><span data-stu-id="dc9c5-101">Installing the Custom Learning Solution Webpart</span></span>

## <a name="prerequisites-for-a-tenant-wide-installation"></a><span data-ttu-id="dc9c5-102">租户范围内安装先决条件</span><span class="sxs-lookup"><span data-stu-id="dc9c5-102">Prerequisites for a tenant-wide installation</span></span>

- <span data-ttu-id="dc9c5-p101">为您的整个租户安装自定义学习 web 部件需要具有 Office 365 管理权限。 如果您没有这些权限，您可以使用 Office 365 管理员或安装的单个网站集的 web 部件。</span><span class="sxs-lookup"><span data-stu-id="dc9c5-p101">To install the Custom Learning webpart for your entire tenant you will need to have Office 365 Administrative permissions.  If you do not have these permissions you can either work with your Office 365 Administrator or install the webpart for an individual site collection.</span></span>
- <span data-ttu-id="dc9c5-105">您或您的 Office 365 管理员必须安装和配置租户范围[应用程序目录](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/set-up-your-developer-tenant)或[网站集应用程序目录](https://docs.microsoft.com/en-us/sharepoint/dev/general-development/site-collection-app-catalog)，以接收 web 部件。]</span><span class="sxs-lookup"><span data-stu-id="dc9c5-105">You or your Office 365 Administrator must have setup and configured a tenant-wide [App Catalog](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/set-up-your-developer-tenant) or a [Site Collection App Catalog](https://docs.microsoft.com/en-us/sharepoint/dev/general-development/site-collection-app-catalog)to receive the webpart.]</span></span>
- <span data-ttu-id="dc9c5-p102">我们仅支持 SharePoint Online。Web 部件不支持任何版本的本地 SharePoint 安装。</span><span class="sxs-lookup"><span data-stu-id="dc9c5-p102">We support SharePoint Online only. The web part is not support for installation on any version of SharePoint on premises.</span></span>

## <a name="add-the-custom-learning-webpart-to-your-tenant"></a><span data-ttu-id="dc9c5-108">将自定义学习 web 部件添加到您的租户</span><span class="sxs-lookup"><span data-stu-id="dc9c5-108">Add the Custom Learning webpart to your tenant</span></span> 

1. <span data-ttu-id="dc9c5-p103">下载自定义学习 web 部件并将其保存到本地驱动器。 此文件被命名为"ms 自定义 learning.sppkg"。 不要更改的名称或文件的后缀。</span><span class="sxs-lookup"><span data-stu-id="dc9c5-p103">Download the Custom Learning webpart and save it to your local drive.  This file is named "ms-custom-learning.sppkg".  Do not change the name or suffix of the file.</span></span> 
2. <span data-ttu-id="dc9c5-112">导航到[Office 365 管理门户](https://admin.microsoft.com/AdminPortal/Home#/homepage)租户</span><span class="sxs-lookup"><span data-stu-id="dc9c5-112">Navigate to the [Office 365 Admin portal](https://admin.microsoft.com/AdminPortal/Home#/homepage) for your tenant</span></span>
3. <span data-ttu-id="dc9c5-p104">左侧导航栏上选择管理中心，SharePoint。这将打开新选项卡中，选择在 SharePoint 管理中心的应用程序、 应用程序目录、 SharePoint 相关应用程序中</span><span class="sxs-lookup"><span data-stu-id="dc9c5-p104">From the left navigation select Admin Centers, SharePoint. This will open in a new tab. , In the SharePoint Admin Center select Apps, App Catalog, Apps for SharePoint</span></span> 
4. <span data-ttu-id="dc9c5-115">选择上载 web 部件，并选择"ms 自定义 learning.sppkg"文件下载</span><span class="sxs-lookup"><span data-stu-id="dc9c5-115">Select upload the webpart and choose the "ms-custom-learning.sppkg" file you downloaded</span></span>
5. <span data-ttu-id="dc9c5-116">为此租户范围内安装检查"使可用于所有此解决方案位于组织中。"旁边的框</span><span class="sxs-lookup"><span data-stu-id="dc9c5-116">For this tenant-wide installation check the box next to "Make this solution available to all sits in the organization."</span></span>  

![部署解决方案](media/trustapp_sm.png)


## <a name="add-the-customer-learning-webpart-to-a-sharepoint-online-page"></a><span data-ttu-id="dc9c5-118">将客户学习 web 部件添加到 SharePoint Online 网页</span><span class="sxs-lookup"><span data-stu-id="dc9c5-118">Add the Customer Learning webpart to a SharePoint Online Page</span></span>

<span data-ttu-id="dc9c5-p105">自定义学习安装在您的租户后您可以向 SharePoint 页面添加 Web 部件。执行操作时，突然 Office 365 培训可供您。</span><span class="sxs-lookup"><span data-stu-id="dc9c5-p105">After Custom Learning is installed in your tenant you can add the Web part to a SharePoint page. When you do, suddenly Office 365 training is available to you.</span></span> 

1. <span data-ttu-id="dc9c5-121">在整个宽度的列布局中添加自定义学习 web 部件：</span><span class="sxs-lookup"><span data-stu-id="dc9c5-121">Add the Custom Learning webpart in a full width column layout:</span></span>

![SharePoint 页面布局](media/clo365fullcolumnwidth.png)

2. <span data-ttu-id="dc9c5-p106">在 SharePoint 页中，选择添加一节，然后选择完整宽度的列。 您将看到以下提示：</span><span class="sxs-lookup"><span data-stu-id="dc9c5-p106">In the SharePoint page, select Add section and then select full width column.  You'll see the following prompt:</span></span>

![AddWebpart](media/clo365addfullwidthwebpart.png)

3. <span data-ttu-id="dc9c5-p107">选择 Microsoft Learning。 您现在应该看到以下：</span><span class="sxs-lookup"><span data-stu-id="dc9c5-p107">Select Microsoft Learning.  You should now see the following:</span></span> 

![学习 web 部件的自定义](media/clo365addwebpart.png)

 <span data-ttu-id="dc9c5-129">您现在可以单击拼贴来分析解决方案中包含的默认内容。</span><span class="sxs-lookup"><span data-stu-id="dc9c5-129">You can now click on the tiles to explore the default content included in the solution.</span></span>  

## <a name="next-steps"></a><span data-ttu-id="dc9c5-130">后续步骤</span><span class="sxs-lookup"><span data-stu-id="dc9c5-130">Next Steps</span></span>
- <span data-ttu-id="dc9c5-131">浏览包括 web 部件中的[默认内容](webpartcontent.md)。</span><span class="sxs-lookup"><span data-stu-id="dc9c5-131">Explore the [default content](webpartcontent.md) included in the webpart.</span></span>
- <span data-ttu-id="dc9c5-132">[自定义](customization.md)您的组织的培训体验。</span><span class="sxs-lookup"><span data-stu-id="dc9c5-132">[Customize](customization.md) the training experience for your organization.</span></span>
- <span data-ttu-id="dc9c5-133">培训解决方案的[驱动器应用](driveadoption.md)。</span><span class="sxs-lookup"><span data-stu-id="dc9c5-133">[Drive adoption](driveadoption.md) of your training solution.</span></span>

