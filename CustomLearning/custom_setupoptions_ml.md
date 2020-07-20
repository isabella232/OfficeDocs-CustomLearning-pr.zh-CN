---
author: pkrebs
ms.author: pkrebs
title: 多语言学习路径的安装选项
ms.date: 07/6/2020
description: 多语言学习路径的安装选项
ROBOTS: NOINDEX, NOFOLLOW
ms.openlocfilehash: 2e2e7a765a7d24ef83a04f0ca3ef6d049cc658e3
ms.sourcegitcommit: 1e6e31d2bd43971b62322c7d2db352961c554d71
ms.translationtype: Auto
ms.contentlocale: zh-CN
ms.lasthandoff: 07/04/2020
ms.locfileid: "45037214"
---
# <a name="setup-options-for-multilingual-learning-pathways"></a>多语言学习路径的安装选项
通过发布 SharePoint Online 通信网站的多语言功能，学习途径现在可支持多种语言。 您可以采用不同类型的方式设置学习路径，以满足组织的需求。 为了帮助您确定组织的最佳路径，我们概述了设置选项。 

## <a name="new-install-scenarios"></a>新安装方案
"新安装方案" 说明了使用 SharePoint 设置服务安装学习路径的新实例的选项现在可以从 SharePoint 的 "查找簿" 中获取。

### <a name="scenario-1-we-have-not-installed-learning-pathways-and-need-learning-pathways-multilingual-support"></a>方案1：我们尚未安装学习路径，需要学习路径多语言支持 
如果尚未安装学习路径，并且需要使用多种语言，则可以使用 SharePoint 设置服务安装具有九种语言支持的新学习路径解决方案。 英语将成为默认语言，无法更改。 
- 若要设置新的学习路径解决方案，将英语用作网站的默认语言，请参阅[设置新的学习路径解决方案](custom_provision_ml.md)。

### <a name="scenario-2-we-installed-learning-pathways-but-arent-currently-using-it-andor-havent-made-any-customization-to-the-site-or-playlists"></a>方案2：我们已安装了学习路径，但当前未使用它，并且/或者尚未对网站或播放列表进行任何自定义 
如果你已安装了学习路径，但未主动使用它，或者尚未对网站或播放列表进行任何自定义，则可以使用 SharePoint 设置服务来安装支持九种语言的新解决方案。 英语将成为默认语言，无法更改。 
- 若要设置新的学习路径解决方案，将英语用作网站的默认语言，请参阅[设置新的学习路径解决方案](custom_provision_ml.md)。

### <a name="scenario-3-we-havent-installed-learning-pathways-and-dont-need-multilingual-support"></a>方案3：我们尚未安装学习路径，也不需要多语言支持 
如果尚未安装学习路径，也不需要多语言支持，可以从 SharePoint 设置服务进行安装。 英语将成为默认语言。 安装完成后，需要关闭多语言支持。 
- 若要设置新的学习路径解决方案而不支持多语言支持，请参阅[设置新的学习路径解决方案](custom_provision_ml.md)。

## <a name="update-learning-pathways-with-a-web-part-upload-scenarios"></a>更新学习路径（使用 web 部件上传）方案
如果已安装学习路径的现有版本，则可以将 "学习路径" web 部件上传到 SharePoint 应用程序目录，以启用多语言支持。 

### <a name="scenario-1-we-need-to-upgrade-an-existing-version-of-learning-pathways-but-dont-need-multilingual-support"></a>方案1：我们需要升级现有版本的学习路径，但不需要多语言支持
您可以更新不带多语言支持的学习路径版本4.0。 通过更新，您可以获得一些新功能，包括自定义播放列表和子类别的图像选择器。 

- 若要更新没有多语言支持的现有学习路径解决方案，请参阅[更新多语言支持的学习路径](custom_update_ml.md)。 无多语言支持的升级过程与多语言支持相同，但步骤较少。 

### <a name="scenario-2-we-need-to-upgrade-to-multilingual-support-and-the-default-language-of-the-site-collection-is-our-default-language"></a>方案2：我们需要升级到多语言支持，网站集的默认语言是我们的默认语言
学习路径版本 4. O 将支持网站集中的多语言页面。 除了多语言支持之外，还可以获取一些新功能，包括用于自定义播放列表和子类别的图像选择器。 
- 若要更新现有学习路径网站的多语言支持，请参阅[更新多语言支持的学习路径](custom_update_ml.md)。 

## <a name="update-learning-pathways-for-multilingual-support-with-manual-install"></a>使用手动安装更新多语言支持的学习途径 
下面概述了将现有的学习路径实例更新为版本4.0 多语言版本的方案，具体方法是手动安装 "学习路径" web 部件。 

### <a name="scenario-1-we-need-multilingual-support-and-the-default-language-of-the-site-collection-is-not-our-default-language--no-custom-content"></a>方案1：我们需要多语言支持，并且网站集的默认语言不是我们的默认语言–无自定义内容 
学习路径版本4.0 将支持此方案。 但是，此方案假定您在现有网站上没有自定义内容或播放列表。 在这种情况下，您可以使用默认语言创建新的 SharePoint Online 通信网站，上载 web 部件，然后使用 PowerShell 脚本手动设置学习路径。 
- 若要设置使用默认语言的多语言支持的学习路径，请参阅[手动安装多语言支持的学习路径](custom_manualsetup_ml.md)。

### <a name="scenario-2-we-need-multilingual-support-and-the-default-language-of-the-site-collection-is-not-our-default-language--plus-we-have-custom-content"></a>方案2：我们需要多语言支持，并且网站集的默认语言不是我们的默认语言–此外还包含自定义内容 
在这种情况下，您可以使用默认语言创建新的 SharePoint Online 通信网站，上载 web 部件，然后使用 PowerShell 脚本手动设置学习路径。 

在您按照上述步骤重新建立学习路径网站后，您需要移动**CustomPlaylists**列表和**CustomAssets**列表的内容。 此外，您还可以在现有的学习路径网站中，移动构成自定义资产的实际自定义页面，并且您的意图是将其删除。 任务可能很困难，因为对于**CustomPlaylists**列表中的所有项， **CustomAssets**列表中的列表项的 ID 将隐藏在每个播放列表项的 JSONData 字段中。 因此，只需将**CustomPlaylists**列表中的内容从一个网站移到另一个网站即可。 此外， **CustomAssets**列表包含列表项的 JSONData 字段中自定义资产页面的绝对 URL。 如果资产未移动，并且网站未重命名（从而将绝对 URL 更改为资产页面），则**CustomAssets**可以保留。 但您需要手动更正这些条目。 考虑到这种类型的迁移的复杂性，我们建议您考虑登记我们的一个学习路径合作伙伴，以帮助您进行此转换。
- 若要设置使用默认语言的多语言支持的学习路径，请参阅[手动安装多语言支持的学习路径](custom_manualsetup_ml.md)。

