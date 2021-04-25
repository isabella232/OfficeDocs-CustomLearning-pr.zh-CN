---
author: pkrebs
ms.author: pkrebs
title: 设置自定义学习网站
ms.date: 02/10/2019
description: 通过 SharePoint 预配引擎预配 Office 365 自定义学习网站
ms.service: sharepoint-online
manager: bpardi
ms.topic: article
audience: admin
ms.openlocfilehash: f930eba5815366bcefd2730c88a3c2df3f246dd4
ms.sourcegitcommit: 97e175e5ff5b6a9e0274d5ec9b39fdf7e18eb387
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/25/2021
ms.locfileid: "52000318"
---
# <a name="provision-custom-learning"></a>预配自定义学习

借助 SharePoint Online 预配服务，Office 365 租户管理员可以通过单击几下即可开始预配过程。 预配服务是设置自定义学习的推荐方法。 它快速、简单，只需几分钟即可开始该过程。 但是，在开始使用预配服务之前，请确保你已满足预配的先决条件。

## <a name="prerequisites"></a>先决条件
 
若要使用设置服务 [SharePoint Online 设置](https://provisioning.sharepointpnp.com)服务成功设置自定义学习，执行预配的人必须满足以下先决条件： 
 
- 预配自定义学习的人必须是将预配自定义学习的租户的租户管理员。  
- 租户应用程序目录必须在 SharePoint 管理中心的"应用程序"选项中提供。 如果您的组织没有 SharePoint 租户应用程序目录，请参阅 [SharePoint Online 文档以](/sharepoint/use-app-catalog) 创建一个。  
- 预配自定义学习的人必须是租户应用程序目录的网站集所有者。 如果预配自定义学习的人不是应用程序目录的网站集所有者，请 [完成这些说明并继续](addappadmin.md) 操作。 

### <a name="to-provision-custom-learning"></a>设置自定义学习

1. 转到 http://provisioning.sharepointpnp.com **，然后** 从主页的右上角登录。  使用计划安装网站模板的目标租户的凭据登录。
![设置服务主页。](media/inst_signin.png)

2. 清除"**代表你的组织同意"，然后选择**"接受 **"。**
![许可屏幕](media/inst_perms.png)

3. 从 **解决方案库中选择"自定义学习 office 365"。**
![选择 Office 365 自定义学习的屏幕。](media/inst_select.png)

4. 在解决方案主页中，选择"**添加到租户** 
 ![ 屏幕"，选择"添加到租户"。](media/inst_add.png)

5. 根据需要填写预配信息页面上的字段。 至少输入要获取预配过程通知的电子邮件地址，以及要预配到的网站的目标 URL。  
   > [!NOTE]
   > 使网站的目标 URL 对员工友好，例如"/sites/MyTraining"或"/teams/LearnOffice365"。

   ![提供预配详细信息的屏幕。](media/inst_options.png)

6. 准备好 **将** 自定义学习安装到租户环境中时，请选择"预配"。  预配流程最多需要 15 分钟。 网站可供访问时，系统将通过电子邮件（你在“预配”页面上输入的通知电子邮件地址）通知你。

> [!IMPORTANT]
> 设置自定义学习网站的租户管理员必须转到该网站，然后打开 CustomLearningAdmin.aspx 以初始化自定义学习管理员属性。 目前，租户管理员还应将所有者分配给网站。 

## <a name="validate-provisioning-success"></a>验证预配成功

预配完成后，租户管理员将收到来自 PnP 预配服务的电子邮件。 管理员可以将链接复制到电子邮件中提供的网站，然后按照说明转到网站。 或者，租户管理员可以导航到 </SitePages/CustomLearningAdmin.aspx>YOUR-SITE-COLLECTION-URL。 这将初始化 CustomConfig 列表项，该列表项将设置自定义学习供其首次使用。 第一次打开此页面的用户必须是租户管理员、网站集管理员或网站所有者。 应看到如下页面： 

## <a name="add-owners-to-site"></a>将所有者添加到网站
作为租户管理员，你不太可能是自定义网站的人，因此你需要将所有者分配给网站。 所有者对网站拥有管理权限，因此可以修改网站页面和重新品牌。 他们还能够隐藏和显示通过自定义学习 Web 部件提供的内容。 他们还可以生成自定义播放列表并将其分配给自定义子类别。  

1. 从"SharePoint **设置"菜单中**，单击"**网站权限"。**
2. 单击 **"高级权限设置"。**
3. 单击 **Office 365 所有者的自定义学习**。
4. 单击 **"**  >  **向此组添加新用户"，** 添加您希望成为所有者的用户，然后单击"共享 **"。**

8. 单击 **页面** 右上角的"关注"选项以关注网站。  
