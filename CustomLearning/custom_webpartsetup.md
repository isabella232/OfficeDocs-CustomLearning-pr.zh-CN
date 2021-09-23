---
author: pkrebs
ms.author: pkrebs
title: 设置自定义Learning网站
ms.date: 02/10/2019
description: 通过 Learning 预配Office 365为网站SharePoint自定义网站
ms.service: sharepoint-online
manager: bpardi
ms.topic: article
audience: admin
ms.openlocfilehash: d8fa6d3c3dbcbcf6c82659e28526bd026c5594e0
ms.sourcegitcommit: a93cae8ea6e3c1141d7266d04131b69f2c2498cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/23/2021
ms.locfileid: "59485220"
---
# <a name="provision-custom-learning"></a>预配自定义Learning

借助 SharePoint Online Provisioning Service，Office 365管理员只需单击几下即可开始预配过程。 预配服务是建议用于预配自定义Learning。 它快速、简单，只需几分钟即可开始该过程。 但是，在开始使用预配服务之前，请确保你已满足预配的先决条件。

## <a name="prerequisites"></a>必备条件
 
若要使用 Learning [Online Provisioning Service](https://provisioning.sharepointpnp.com)成功设置自定义SharePoint服务，执行预配的人必须满足以下先决条件： 
 
- 预配自定义Learning必须是将预配自定义租户的租户Learning管理员。  
- 租户应用程序目录必须在管理中心的"应用程序"选项SharePoint可用。 如果你的组织没有租户应用SharePoint目录，请参阅 SharePoint [Online 文档](/sharepoint/use-app-catalog)创建一个。  
- 预配自定义网站Learning必须是租户应用程序目录的网站集所有者。 如果预配自定义Learning不是应用程序目录的网站集所有者，请[完成这些](addappadmin.md)说明并继续操作。 

### <a name="to-provision-custom-learning"></a>设置自定义Learning

1. 转到 http://provisioning.sharepointpnp.com **，然后** 从主页的右上角登录。  使用计划安装网站模板的目标租户的凭据登录。
![设置服务主页。](media/inst_signin.png)

2. 清除"**代表你的组织同意"，然后选择**"接受 **"。**

   ![安装权限](media/inst_perms.png)

3. 从 **解决方案Learning选择Office 365** 自定义模板" 。
![屏幕，选择自定义Learning自定义Office 365。](media/inst_select.png)

   ![安装选项选择](media/inst_select.png)

4. 从解决方案主页选择" **添加到租户"**

      ![inst_select.png](media/inst_add.png)

5. 根据需要填写预配信息页面上的字段。 至少输入要获取预配过程通知的电子邮件地址，以及要预配到的网站的目标 URL。  
   > [!NOTE]
   > 使网站的目标 URL 对员工友好，例如"/sites/MyTraining"或"/teams/LearnOffice365"。

   ![安装选项](media/inst_options.png)

6. 准备好 **在** 租户环境中安装自定义Learning选择预配。  预配流程最多需要 15 分钟。 网站可供访问时，系统将通过电子邮件（你在“预配”页面上输入的通知电子邮件地址）通知你。

> [!IMPORTANT]
> 设置自定义网站Learning管理员必须转到该网站，然后打开 CustomLearningAdmin.aspx 以初始化自定义Learning管理员属性。 目前，租户管理员还应将所有者分配给网站。 

## <a name="validate-provisioning-success"></a>验证预配成功

预配完成后，租户管理员将收到来自 PnP 预配服务的电子邮件。 管理员可以将链接复制到电子邮件中提供的网站，然后按照说明转到网站。 或者，租户管理员可以导航到 YOUR-SITE-COLLECTION-URL/SitePages/CustomLearningAdmin.aspx。 这将初始化 CustomConfig 列表项，该列表项设置自定义Learning首次使用。 第一次打开此页面的用户必须是租户管理员、网站集管理员或网站所有者。 应该会看到如下页面： 

## <a name="add-owners-to-site"></a>将所有者添加到网站
作为租户管理员，你不太可能是自定义网站的人，因此你需要将所有者分配给网站。 所有者对网站拥有管理权限，因此可以修改网站页面和重新品牌。 他们还能够隐藏和显示通过自定义自定义 Web 部件Learning的内容。 他们还可以生成自定义播放列表并将其分配给自定义子类别。  

1. 从 **"SharePoint设置"** 菜单中，单击"**网站权限"。**
2. 单击 **"高级权限设置"。**
3. 单击 **适用于 Office 365 的自定义学习所有者"。**
4. 单击 **"**  >  **向此组添加新用户"，** 添加您希望成为所有者的用户，然后单击"共享 **"。**

8. 单击 **页面** 右上角的"关注"选项以关注网站。  
