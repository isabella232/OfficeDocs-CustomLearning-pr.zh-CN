---
author: karuanag
ms.author: karuanag
manager: alexb
title: 自定义和共享播放列表
ms.date: 02/10/2019
description: 从现有内容或新 SharePoint 页面创建自定义播放列表
ms.service: sharepoint-online
audience: itpro
ms.topic: article
ms.openlocfilehash: 31a0e5524181d26f4d62ae7206636c9e553b6f8f
ms.sourcegitcommit: 97e175e5ff5b6a9e0274d5ec9b39fdf7e18eb387
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/25/2021
ms.locfileid: "52000208"
---
# <a name="customize-and-share-playlists"></a>自定义和共享播放列表

## <a name="create-a-playlist"></a>创建播放列表

播放列表是"资产"的一个复杂过程。 "资产"是 SharePoint 页面或 Microsoft 培训内容的现有项。 创建播放列表时，选择一起为用户创建学习路径的资产。  

添加 SharePoint 页面的好处是，您可以使用组织中托管的 YouTube 视频创建 SharePoint 页面。 您还可以使用 Forms 或其他 Office 365 内容创建页面。  

#### <a name="step-1-create-a-sharepoint-page-for-your-playlist"></a>步骤 1：为播放列表创建 SharePoint 页面
此示例首先创建一个要添加到播放列表的 SharePoint 页面。 我们将创建一个包含 YouTube 视频 Web 部件和文本 Web 部件的页面。  这些说明假定你使用的是 SharePoint Online 服务。 

#### <a name="create-a-new-page"></a>创建新页面
1.  Select the Settings menu > Site Contents > Site Pages > New > Site Page.
2.  在标题区域中，键入使用 Teams 命令框
3.  选择"添加新节"，然后选择"两列"。

![两列添加](media/clo365addtwocolumn.png)

4.  在左侧框中，选择"添加新 Web 部件"，然后选择"嵌入"。 
5.  在 Web 浏览器中，转到此 URL https://youtu.be/wYrRCRphrp0 并获取视频的嵌入代码。 
6.  在 SharePoint Web 部件中，选择"添加嵌入代码"，然后将其粘贴到"嵌入"框中。 
7.  在右侧框中，选择"添加新 Web 部件"，然后选择"文本"。 
8.  在 Web 浏览器中，转到此 URL： https://support.office.com/article/13c4e429-7324-4886-b377-5dbed539193b 并复制试用！ 页面中的说明，并将其粘贴到文本 Web 部件中。 页面应如下所示。 
![嵌入页面](media/clo365teamscommandbox.png)
9.  单击 **"** 发布"，然后复制页面的 URL 并将其粘贴到记事本中

#### <a name="step-2-create-the-playlist"></a>步骤 2：创建播放列表

1. 导航到 **网站体验中的** "自定义学习管理"页。
![选择"自定义学习管理"的屏幕。](media/custom_admin.png)
1. 确保 **已选择** "类别" 
1. 单击要显示新播放列表的类别
1. 在类别名称旁边，单击加号"窗口"，并突出显示 ![ "类别"选项和"加号"。](media/custom_addplay.png)

1. 填写值，如下面的示例所示， **然后选择创建**。 
![输入播放列表详细信息的页面。](media/custom_details.png)
- **Title** - 播放列表的显示名称
- **说明** - 将学习哪些内容的信息
- **类别** - 根据初始选择预选
- **子类别** - 根据你的选择预选
- **技术** - 选择（如果适用）
- **Level** - 初学者、Intermidate 或 Advanced
- **访问** 群体 - 这允许您基于 Microsoft 提供的角色的预定义列表来定位内容。

6. 单击 **"保存详细信息"**

> [!TIP]
> 你可以自定义播放列表的图标图像。  单击图像图标并插入以前上载的图像的 URL。  确保图像位于自定义学习网站集内或所有用户都将有权访问该文件的另一个位置。  
![选择图像窗口。](media/custom_image.png)

#### <a name="step-3-add-assets-to-the-playlist"></a>步骤 3：将资产添加到播放列表
在此步骤中，你将从 Microsoft 和你创建的 SharePoint 页面将现有资源添加到播放列表。 

1. 保存播放列表的详细信息后，可以使用"搜索现有资源"。
1. **输入任何搜索词** 以查看可从其他播放列表访问的预定义资产列表。 **单击资产名称** 以将资产添加到新播放列表中。<br/>
![播放列表资产页面](media/custom_slist.png)

还可以添加之前创建的 SharePoint 页面，或从头开始创建一个体验页面。

1. 单击" **播放列表资产"** 对话框中的"新建资产"选项。
1. 为资产提供 **标题**。 输入后，将显示其他选项。
![输入标题和其他详细信息的表单。](media/custom_newpage.png)
1. 现在可以在 SharePoint Online 中创建新的资产页面，或输入现有页面的 URL 以将其添加到自定义播放列表。 
1. **"****类别"、"** 子类别"和"技术"字段将基于你之前对此播放列表的选择进行预填充。 
1. 为此单个资产的"级别"和"访问群体"进行适当的选择。  
1. 单击 **"保存资产** "将其添加到自定义播放列表
1. 重复这些步骤（搜索或添加单个页面）直到播放列表完成。 
1. 单击 **关闭播放列表** 以保存

你具有此内容的播放列表现在将在你已安装/嵌入自定义学习 Web 部件的任何位置可用。 

> [!NOTE]
> 如果在关闭播放列表后出错，可以通过单击播放列表名称旁边的 X 将其从类别中删除。  

#### <a name="things-to-think-about"></a>要思考的事情

自定义播放列表可用于帮助最终用户完成各种任务。  您是否有请假请求表单？  请求硬件设备的表单  可以将任何现有培训资产编入体验。  

## <a name="share-playlists"></a>共享播放列表

1. 导航到 Web 部件或网站体验内的任何播放列表
1. 在左上角，你将看到三个图标
1. 单击表示链接的图标
1. 将 URL 复制到播放列表 ![ 屏幕，单击 URL 旁边的"复制"。](media/share.png)
现在可以在网站导航中插入此 URL，或在其他通信中利用此 URL 将员工直接添加到该播放列表中。 

### <a name="next-steps---drive-adoption"></a>下一步 - [推动采用](driveadoption.md)
