---
author: pkrebs
ms.author: pkrebs
title: 预配自定义学习网站
ms.date: 02/10/2019
description: 通过 SharePoint 预配引擎为 Office 365 网站设置自定义学习
ms.service: sharepoint online
ms.openlocfilehash: feebef7f351aab4cd1efe7f87596dad98dba7536
ms.sourcegitcommit: ee4aebf60893887ae95a1294a9ad8975539ea762
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/23/2020
ms.locfileid: "48233754"
---
# <a name="provision-custom-learning"></a>预配自定义学习

借助 SharePoint Online 设置服务，Office 365 租户管理员可以通过几次简单的单击操作来启动预配过程。 预配服务是设置自定义学习的推荐方法。 快速而简单，只需几分钟即可启动该过程。 但是，在开始使用预配服务之前，请确保已满足预配的先决条件。

## <a name="prerequisites"></a>先决条件
 
若要使用预配服务 [SharePoint Online 设置服务](https://provisioning.sharepointpnp.com)成功设置自定义学习，进行预配的人员必须满足以下先决条件： 
 
- 人员预配自定义学习必须是租户 Administratorof 租户，在此租户中将预配自定义学习。  
- 租户应用程序目录必须在 SharePoint 管理中心的 "应用程序" 选项中可用。 如果您的组织没有 SharePoint 租户应用程序目录，请参阅 [SharePoint Online 文档](https://docs.microsoft.com/sharepoint/use-app-catalog) 以创建一个。  
- 人员预配自定义学习必须是租户应用程序目录的网站集所有者。 如果人员预配自定义学习不是应用程序目录的网站集所有者，请 [完成这些说明](addappadmin.md) 并继续。 

### <a name="to-provision-custom-learning"></a>预配自定义学习

1. http://provisioning.sharepointpnp.com从主页的右上角转到并**登录**。  使用您计划安装网站模板的目标租户的凭据登录。

![pnphome.png](media/inst_signin.png)

2. 清除 **代表您的组织的同意** 并选择 " **接受**"。

![实时](media/inst_perms.png)

3. 从解决方案库中选择 **适用于 Office 365 的自定义学习** 。

![实时](media/inst_select.png)

4. 从解决方案主页中选择 "**添加到你的租户**"

![inst_select.png](media/inst_add.png)

5. 根据需要填写预配信息页面上的字段。 至少应输入你希望获取有关设置过程的通知的电子邮件地址和要设置为的网站的目标 URL。  
> [!NOTE]
> 将网站的目标 URL 设置为友好的内容，如 "/sites/MyTraining" 或 "/teams/LearnOffice365"。

![inst_options.png](media/inst_options.png)

6. 准备好将自定义学习安装到租户环境中时，请选择 " **设置** "。  预配流程最多需要 15 分钟。 网站可供访问时，系统将通过电子邮件（你在“预配”页面上输入的通知电子邮件地址）通知你。

> [!IMPORTANT]
> 设置自定义学习网站的租户管理员必须转到网站，然后打开 CustomLearningAdmin 以初始化自定义学习管理属性。 目前，租户管理员还应将所有者分配给网站。 

## <a name="validate-provisioning-success"></a>验证设置是否成功

设置完成后，租户管理员将从 PnP 预配服务收到电子邮件。 管理员可以将链接复制到电子邮件中提供的网站，然后按照说明转到网站。 此外，租户管理员还可以导航到 <您的网站集 URL>/SitePages/CustomLearningAdmin.aspx。 这将初始化为其首次使用设置自定义学习的 CustomConfig 列表项。 首次打开此页面的人员必须是网站的租户管理员、网站集管理员或所有者。 您应该会看到如下所示的页面： 

## <a name="add-owners-to-site"></a>将所有者添加到网站
作为租户管理员，您不太可能是自定义网站的人，因此您需要将所有者分配到网站。 所有者具有对网站的管理权限，以便他们可以修改网站页面并 rebrand 网站。 他们还能够隐藏和显示通过自定义学习 Web 部件传递的内容。 他们还能够构建自定义播放列表并将其分配给自定义子类别。  

1. 从 "SharePoint **设置** " 菜单中，单击 " **网站权限**"。
2. 单击 " **高级权限设置**"。
3. 单击 " **自定义学习 For Office 365 所有者**"。
4. 单击 "**新建**向  >  **此组添加用户**"，添加您希望成为所有者的人员，然后单击 "**共享**"。

8. 单击页面右上角的 **以下** 选项以关注网站。  

### <a name="next-steps"></a>后续步骤
- 浏览 web 部件中包含的 [默认内容](sitecontent.md) 。
