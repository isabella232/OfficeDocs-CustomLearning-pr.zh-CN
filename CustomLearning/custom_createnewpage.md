---
author: pkrebs
ms.author: pkrebs
title: 为播放列表创建 SharePoint 页面
ms.date: 02/10/2019
description: 为播放列表创建 SharePoint 页面
ms.service: sharepoint online
ms.openlocfilehash: 99425b9be685a8090394ecb446a7c82dee24fe5d
ms.sourcegitcommit: ee4aebf60893887ae95a1294a9ad8975539ea762
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/23/2020
ms.locfileid: "48234504"
---
# <a name="create-sharepoint-pages-for-custom-playlists"></a>为自定义播放列表创建 SharePoint 页面

学习路径的独特功能之一是能够创建从 Microsoft 的资产和您创建的 SharePoint 资产汇编的播放列表。 在此示例中，我们将事先创建一个 SharePoint 页来创建播放列表。 通过 SharePoint 页面构建播放列表的功能可提供多种机会，以使用 Microsoft 或你的组织提供的 Web 部件构建页面。 例如，播放列表可以包括 SharePoint 页面，其中包含来自 YouTube 的嵌入式视频，或从 Office 365 表单或嵌入的 Power BI 报表生成的表单。 在此示例中，我们将介绍如何使用 "嵌入 web 部件" 和 "文本" web 部件生成页面。  

## <a name="create-a-sharepoint-page-for-a-custom-playlist"></a>为自定义播放列表创建 SharePoint 页面

1. 单击 "SharePoint **齿轮** " 图标，然后单击 " **添加页面**"。
2. 单击页面左侧的 " **添加新内容 (+) ** "，然后单击 " **两列** " 以查看分区布局。
3. 在左侧列中，单击 "+"，然后单击 " **嵌入** web 部件"。 
4. 在右列中，单击 "+"，然后单击 " **文本** " web 部件。 页面应如下所示。

![cg-pagenewstart.png](media/cg-pagenewstart.png)

### <a name="add-a-video-and-text-from-youtube"></a>从 YouTube 添加视频和文本

1. 在浏览器中，转到 "YouTube"。 对于此示例，请搜索 "什么是 Office 365 – Microsoft 的最佳生产力应用程序"。
2. 单击视频进行播放，然后将其暂停，然后右键单击该视频。 
3. 单击 " **复制嵌入代码**"，然后返回到 "SharePoint" 页面。 
4. 单击 "**嵌入**web 部件" 中的 "**添加嵌入代码**"，然后添加 YouTube 视频中的代码。
5. 返回到 YouTube 页面，并复制视频的 **说明** 文本。 
6. 返回到 "SharePoint" 页面，选择 " **文本** " web 部件，然后复制 YouTube 视频中的文本。
7. 在 SharePoint 页面的 "标题" 区域中选择 " **编辑 web 部件** " 图标，然后将该页面命名为 "自定义播放列表简介"。 
8. 对于 " **布局**"，选择 " **无**"，然后关闭 " **标题区域** 属性" 窗格。 此时，页面应类似于以下内容。 

![cg-pagenewfinish.png](media/cg-pagenewfinish.png)

### <a name="publish-the-page"></a>发布页面

- 选择 " **发布** " 按钮。 现在，你已准备好将此 SharePoint 页面添加到自定义播放列表中。 