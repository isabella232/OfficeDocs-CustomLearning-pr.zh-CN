---
author: pkrebs
ms.author: pkrebs
title: 为播放列表创建 SharePoint 页面
ms.date: 02/10/2019
description: 为播放列表创建 SharePoint 页面
ms.service: sharepoint-online
ms.openlocfilehash: 40c249fbd5b0fdaefd555f23bf20ac23240ea954
ms.sourcegitcommit: 97e175e5ff5b6a9e0274d5ec9b39fdf7e18eb387
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/25/2021
ms.locfileid: "51999083"
---
# <a name="create-sharepoint-pages-for-custom-playlists"></a>为自定义播放列表创建 SharePoint 页面

学习路径的独特功能之一是能够创建从 Microsoft 的资产和您创建的 SharePoint 资产汇编的播放列表。 本示例中，我们将先创建一个 SharePoint 页面，再创建一个播放列表。 通过 SharePoint 页面生成播放列表的能力提供了使用 Microsoft 或组织提供的 Web 部件生成页面的各种机会。 例如，播放列表可以包括 SharePoint 页面（包含 YouTube 中的嵌入视频）或从 Office 365 Forms 构建的表单或嵌入的 Power BI 报表。 本示例将展示如何使用嵌入 Web 部件和文本 Web 部件生成页面。  

## <a name="create-a-sharepoint-page-for-a-custom-playlist"></a>为自定义播放列表创建 SharePoint 页面

1. 单击"SharePoint **齿轮**"图标，然后单击"**添加页面"。**
2. 单击 **页面左侧的**" (+) "，然后单击"两列"作为该节布局。 
3. 在左侧列中，单击"+"，然后单击" **嵌入** Web 部件"。 
4. 在右侧列中，单击"+"，然后单击"文本 **"Web** 部件。 你的页面应如下所示。

![cg-pagenewstart.png](media/cg-pagenewstart.png)

### <a name="add-a-video-and-text-from-youtube"></a>从 YouTube 添加视频和文本

1. 在浏览器中，转到 YouTube。 对于此示例，搜索"什么是 Office 365 – Microsoft 的最佳生产力应用"。
2. 单击视频以播放它，然后暂停它，然后右键单击它。 
3. 单击 **"复制嵌入代码**"，然后返回到 SharePoint 页面。 
4. 单击 **"在嵌入** Web **部件中添加** 嵌入代码"，然后从 YouTube 视频添加代码。
5. 返回到 YouTube 页面并复制 **视频的说明** 文本。 
6. 返回到 SharePoint 页面，选择 **"文本** "Web 部件，然后从 YouTube 视频复制文本。
7. 选择 **SharePoint** 页面的"标题"区域中的"编辑 Web 部件"图标，然后将页面命名为"自定义播放列表简介"。 
8. 对于 **"布局"，****选择"纯**"，然后关闭 **"标题区域** 属性"窗格。 现在，页面应如下所示。 

![cg-pagenewfinish.png](media/cg-pagenewfinish.png)

### <a name="publish-the-page"></a>发布页面

- 选择" **发布"** 按钮。 现在，你已准备好将此 SharePoint 页面添加到你的自定义播放列表。 