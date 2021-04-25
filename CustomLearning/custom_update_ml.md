---
author: pkrebs
ms.author: pkrebs
title: 更新多语言支持的学习路径
ms.date: 05/20/2019
description: 更新多语言支持的学习路径
ROBOTS: NOINDEX, NOFOLLOW
ms.service: sharepoint-online
manager: bpardi
ms.topic: article
audience: admin
ms.openlocfilehash: 9344cd91e5b6718b1eb0e73e25fdc8311afed793
ms.sourcegitcommit: 97e175e5ff5b6a9e0274d5ec9b39fdf7e18eb387
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/25/2021
ms.locfileid: "52000238"
---
# <a name="update-learning-pathways-for-multilingual-support"></a>更新多语言支持的学习路径
如果你有一个现有的学习路径网站，你可以更新它，实现多语言支持。 若要更新多语言 4.0 版本的学习路径，需要将 Web 部件包 customlearning.sppkg 上载到 SharePoint 租户应用程序目录。 更新学习路径时：  

- 保留以前创建的任何自定义播放列表和资产
- 用于隐藏或显示内容的设置将保留
- SharePoint 模板的学习路径保持不变
- 不会翻译学习路径网站页面。 必须手动完成此工作

## <a name="read-the-learning-pathways-multilingual-overview"></a>阅读学习路径多语言概述
若要了解多语言支持如何用于学习路径，请阅读学习路径 [多语言概述](custom_overview_ml.md)) 。 

## <a name="prerequisites-to-update"></a>更新的先决条件
在更新学习路径之前，必须满足以下先决条件：
- 更新学习路径的人必须是租户应用程序目录的网站集所有者。 如果预配学习路径的人不是应用程序目录的网站集所有者，请 [完成这些](addappadmin.md) 说明并继续操作。 

## <a name="set-language-settings"></a>设置语言设置 
在更新学习路径之前，请设置网站语言设置。 若要启用对学习路径网站的多语言支持，可以将"允许将页面和新闻翻译为多种语言"设置为 **"** 打开"，然后添加要支持该网站的语言。
1.  从"学习路径"网站中，**从右** 上方选择"设置"，然后选择"网站 **信息"。**
2.  在网站信息窗格底部，选择"**查看所有网站设置"。**
3.  在 **"网站管理"下**，选择"**语言设置"。**
4.  在 **"启用要翻译为多种语言的页面** 和新闻"下，设置切换开关。 
- 对于多语言网站，将开关滑动到 **"打开**"，然后继续"添加语言"部分。 
- 对于仅英文网站，将切换开关滑动到 **"关"。**

### <a name="add-languages"></a>添加语言
学习路径支持九种语言，应仅添加所需的语言。 在本文档中使用的示例中，将添加意大利语。 
- 在 **"添加或删除网站语言"下**，开始在"选择或键入语言"中键入语言名称，或者从下拉列表中选择语言。 可以重复此步骤以添加多种语言。 通过返回到此页面，您随时都可以在网站中添加或删除语言。
 
### <a name="assign-translators"></a>分配翻译人员
定义学习路径的语言设置时，可以分配翻译人员。 翻译人员应设置外语配置文件。 有关外语配置文件的信息，请参阅创建 [多语言通信网站、页面和新闻](https://support.office.com/article/2bb7d610-5453-41c6-a0e8-6f40b3ed750c)。  
- 对于受支持的语言，请单击 **"选择或键入转换器** "，然后选择一个转换器。 

## <a name="update-the-learning-pathways-web-part-package"></a>更新学习路径 Web 部件包
在此步骤中，您将学习路径 4.0 Web 部件上载到 SharePoint 应用程序目录，然后导航到学习路径管理页以开始更新过程。

### <a name="upload-the-web-part-package"></a>上传 Web 部件包
1.  转到 [GitHub 自定义学习存储库](https://github.com/pnp/custom-learning-office-365/tree/master/webpart)，选择 **customlearning.sppkg，** 然后将它下载到电脑上的本地驱动器。 
2.  如果你尚未登录，请使用租户管理员或网站集管理员帐户登录租户。 
3.  单击 **"管理员**  >  **显示**  >  **所有 SharePoint**  >  **更多功能"。** 
4.  在"**应用"** 下，单击"**打开"。** 
5.  单击 **"应用程序目录**  >  **分发 SharePoint 应用程序"。** 
6.  单击 **上传**  >  **选择文件**。 
7.  选择已 **下载的 customlearning.sppkg** 文件，**单击"确定**""部署  >  **"。** 

### <a name="complete-the-update"></a>完成更新
1.  从"学习路径"网站，从"开始" **菜单中选择** "学习路径 **管理** "。 
2.  你将看到一条提示，询问是否要更新。 
![custom_update_adminprompt_ml.png](media/custom_update_adminprompt_ml.png)
3.  单击“**开始**”。 
4. 更新完成后，单击 **关闭。** 

### <a name="next-steps"></a>后续步骤
- 浏览 [网站和](custom_exploresite.md) Web 部件中提供的默认内容。
- 有关翻译网站页面的信息，请参阅翻译 [网站页面](custom_translate_page_ml.md)。 

