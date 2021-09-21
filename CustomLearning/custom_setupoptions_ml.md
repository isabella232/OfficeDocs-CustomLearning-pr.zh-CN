---
author: pkrebs
ms.author: pkrebs
title: 多语言学习路径的设置选项
ms.date: 07/6/2020
description: 多语言学习路径的设置选项
ROBOTS: NOINDEX, NOFOLLOW
ms.service: sharepoint-online
manager: bpardi
ms.topic: article
audience: admin
ms.openlocfilehash: b4f5b569e7c8395deaea8c436577fb630bce0668
ms.sourcegitcommit: 6005c2551bdea334767e6a056fdcb79533f2c858
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/21/2021
ms.locfileid: "59461161"
---
# <a name="setup-options-for-pathways-for-multilingual-learning"></a>多语言学习路径的设置选项
随着针对联机通信网站的多语言功能SharePoint，学习路径现在支持多种语言。 您可以以不同类型的方式设置学习路径，以满足组织的需求。 为了帮助你确定最适合贵组织的路径，我们概述了设置选项。 

## <a name="new-install-scenarios"></a>新的安装方案
"新安装方案"介绍了使用 SharePoint 设置服务安装学习路径的新实例的选项，现在可从 SharePoint书获得。

### <a name="scenario-1-we-have-not-installed-learning-pathways-and-need-learning-pathways-multilingual-support"></a>方案 1：我们尚未安装学习路径，并且需要学习路径多语言支持 
如果尚未安装学习路径并需要多种语言，可以使用 SharePoint Provisioning Service 安装支持 9 种语言的新学习路径解决方案。 英语将是默认语言，不能更改。 
- 若要设置新的学习路径解决方案，将英语作为网站的默认语言，请参阅预配 [新的学习路径解决方案](custom_provision_ml.md)。

### <a name="scenario-2-we-installed-learning-pathways-but-arent-currently-using-it-andor-havent-made-any-customization-to-the-site-or-playlists"></a>方案 2：我们安装了学习路径，但当前没有使用它和/或尚未对站点或播放列表进行任何自定义 
如果你安装了学习路径，但没有主动使用它，或者你尚未对站点或播放列表进行任何自定义，可以使用 SharePoint 预配服务安装支持九种语言的新解决方案。 英语将是默认语言，不能更改。 
- 若要设置新的学习路径解决方案，将英语作为网站的默认语言，请参阅预配 [新的学习路径解决方案](custom_provision_ml.md)。

### <a name="scenario-3-we-havent-installed-learning-pathways-and-dont-need-multilingual-support"></a>方案 3：我们尚未安装学习路径，也不需要多语言支持 
如果尚未安装学习路径并且不需要多语言支持，可以从 SharePoint 设置服务进行安装。 英语将是默认语言。 安装后，需要关闭多语言支持。 
- 若要设置没有多语言支持的新学习路径解决方案，请参阅预配 [新的学习路径解决方案](custom_provision_ml.md)。

## <a name="update-learning-pathways-with-a-web-part-upload-scenarios"></a>使用 Web 部件 (更新学习路径) 应用场景
如果已安装现有版本的学习路径，可以将学习路径 Web 部件上载到 SharePoint 应用程序目录，以支持多语言支持。 

### <a name="scenario-1-we-need-to-upgrade-an-existing-version-of-learning-pathways-but-dont-need-multilingual-support"></a>方案 1：我们需要升级现有版本的学习路径，但不需要多语言支持
你可以更新学习路径版本 4.0，而无需多语言支持。 通过更新，你可以获取一些新功能，包括自定义播放列表和子类别的图像选择器。 

- 若要更新没有多语言支持的现有学习路径解决方案，请参阅 [更新多语言支持的学习路径](custom_update_ml.md)。 无多语言支持的升级过程与多语言支持相同，但步骤较少。 

### <a name="scenario-2-we-need-to-upgrade-to-multilingual-support-and-the-default-language-of-the-site-collection-is-our-default-language"></a>方案 2：我们需要升级到多语言支持，网站集的默认语言是默认语言
Learning 4.O 版本支持网站集中的多语言页面。 除了多语言支持，你还有一些新功能，包括自定义播放列表和子类别的图像选择器。 
- 若要更新现有学习路径网站多语言支持，请参阅 [更新多语言支持的学习路径](custom_update_ml.md)。 

## <a name="update-learning-pathways-for-multilingual-support-with-manual-install"></a>通过手动安装更新多语言支持的学习路径 
下面概述了通过手动安装学习路径 Web 部件将学习路径解决方案的现有实例更新到 4.0 多语言版本的方案。 

### <a name="scenario-1-we-need-multilingual-support-and-the-default-language-of-the-site-collection-is-not-our-default-language--no-custom-content"></a>方案 1：我们需要多语言支持，网站集的默认语言不是我们的默认语言，没有自定义内容 
Learning 4.0 版支持此方案。 但是，此方案假定你对现有网站没有自定义内容或播放列表。 对于此方案，可以使用默认语言新建 SharePoint Online 通信网站，上载 Web 部件，然后使用 PowerShell 脚本手动设置学习路径。 
- 若要使用默认语言设置多语言支持的学习路径，请参阅手动安装多语言Learning[路径](custom_manualsetup_ml.md)。

### <a name="scenario-2-we-need-multilingual-support-and-the-default-language-of-the-site-collection-is-not-our-default-language--plus-we-have-custom-content"></a>方案 2：我们需要多语言支持，网站集的默认语言不是我们的默认语言 ，而且我们还有自定义内容 
对于此方案，可以使用默认语言新建 SharePoint Online 通信网站，上载 Web 部件，然后使用 PowerShell 脚本手动设置学习路径。 

按照上述步骤重新建立学习路径网站后，需要移动 **CustomPlaylists** 列表和 **CustomAssets 列表** 的内容。 如果自定义资产位于现有学习路径网站中，则还可以移动实际自定义页面（如果它们位于现有学习路径网站中，并且您打算将其删除）。 任务可能比较困难，因为对于 **CustomPlaylists** 列表中的所有项 **，CustomAssets** 列表中的列表项的 ID 将隐藏在每个播放列表列表项的 JSONData 字段中。 因此，仅将 **CustomPlaylists** 列表的内容从一个网站移动到另一个网站是不够的。 此外 **，CustomAssets** 列表包含列表项的 JSONData 字段中自定义资产页面的绝对 URL。 如果未移动资产，并且网站未重命名 (因此将绝对 URL 更改到资产的页面) ， **则 CustomAssets** 可以保留。 但需要手动更正条目。 鉴于这种类型的迁移的复杂性，我们建议你考虑招募我们的学习路径合作伙伴之一来帮助你进行此过渡。
- 若要使用默认语言设置多语言支持的学习路径，请参阅手动安装多语言Learning[路径](custom_manualsetup_ml.md)。

