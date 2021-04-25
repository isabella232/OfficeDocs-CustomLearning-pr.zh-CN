---
author: pkrebs
ms.author: pkrebs
title: 合作伙伴集成模型
ms.date: 3/9/2019
description: 合作伙伴集成模型
ms.service: sharepoint-online
manager: bpardi
ms.topic: article
audience: admin
ms.openlocfilehash: 826b8a463fde50188abbc80e295924b120104cf6
ms.sourcegitcommit: 97e175e5ff5b6a9e0274d5ec9b39fdf7e18eb387
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/25/2021
ms.locfileid: "51999518"
---
# <a name="partner-integration-models"></a>合作伙伴集成模型
虽然无法直接从 SharePoint Online 预配服务"开箱即用"补充 Microsoft 365 学习路径内容，但合作伙伴可以利用多种集成模型来创建一致的增值服务产品。 以上合作伙伴集成模型按复杂性和投资级别的升序呈现。 因此，我们的指南是基于你的业务模型构建你的专长并培养到更高级的级别。

![流程图显示启用者、集成商和重新分发者的角色。](media/cg-part-intmodel.png)

## <a name="how-should-i-get-started"></a>如何开始使用？ 
To get started， here are some best practices to follow.     

### <a name="1-begin-with-building-expertise-as-an-enabler"></a>1. 首先构建作为启用者的专业知识。 
通过启用他们学习路径培训门户并执行有针对性的 Microsoft 内容库，你可以帮助一定比例的客户。 有关设置学习路径的说明，请参阅 https://docs.microsoft.com/office365/customlearning/custom_provision 。  

### <a name="2-then-extend-your-services-as-an-integrator"></a>2. 然后将服务扩展为集成商
执行投资分析的自动化返回 - 具体取决于内容和/或服务集成需求的数量。 例如，如果你可以快速手动创建指向付费内容的目标自定义播放列表 () 或引用你的服务，那么根据我们的内容集成指南，承担开发和运营成本可能没有意义。

### <a name="3-when-the-return-on-investment-makes-sense--consider-redistribution"></a>3. 当投资回报有意义时 – 考虑重新分发 
当投资回报有意义时 – 考虑重新分发 (或与合作伙伴合作，) 重新打包的解决方案。 这些基于 SharePoint 模式和做法框架，该框架提供用于提取自定义网站然后部署到客户环境的解决方案 

## <a name="partner-provided-content-integration-guidelines"></a>合作伙伴提供的内容集成指南
Microsoft 365 学习路径的内容由一组 JSON 文件驱动，这些文件充当学习包的内容清单。 有三个文件：打开metadata.js打开playlists.js打开，assets.js打开。 这些文件需要结构化以匹配 Web 部件识别的模型，然后从内容交付网络 (CDN) 托管，以允许 Web 部件加载它们。 Microsoft 将提供这些文件的起始模板，以便你入门。  

**免责声明：JSON** 文件结构可能会根据即将推出的解决方案工作发生变化。 Microsoft 365 学习路径合作伙伴 Early Adopter program (EAP) 将告知他们任何即将发生的此特性变化。 以及任何客户向后兼容性和/或转换指南。 

### <a name="download-the-microsoft-365-learning-pathways-solution"></a>下载 Microsoft 365 学习路径解决方案
可以从 GitHub 存储库下载 Microsoft 365 学习路径解决方案以及 JSON 文件 https://github.com/pnp/custom-learning-office-365 ：。 请注意，目前 Microsoft 不会对解决方案提出 GitHub 拉取请求。 但是，可以将 GitHub 文件用作创建自己的自定义内容包的起点。 

### <a name="metadatajson-structure"></a>Metadata.js结构
你可以将此文件视为菜单和结构的一部分。 它包含所有导航结构以及选取其他两个文件中数据的列表。 


|              名称        |                     说明                                                               | 
|:-----------------------------|-------------------------------------------------------------------------------------------|
|**技术**              |内容已标记，并且可基于所分配的技术隐藏。                 |  
|&nbsp;&nbsp;Id                |表示技术的 GUID                                                           |  
|&nbsp;&nbsp;名称              |技术的显示名称                                                             |
|&nbsp;&nbsp;*主题[ ]*     |作为技术的子集的主题数组                                   | 
|&nbsp;&nbsp;&nbsp;&nbsp;Id    |表示主题的 GUID                                                              |
|&nbsp;&nbsp;&nbsp;&nbsp;名称  |主题的显示名称                                                                |
|**Categories [ ]**             |类别通知 Web 部件导航。 每个类别表示导航的顶级                                                                                                                 |
|&nbsp;&nbsp;Id                |表示类别/子类别的 GUID                                                 |
|&nbsp;&nbsp;名称              |类别/子类别的显示名称                                                  |
|&nbsp;&nbsp;图像             |应显示在 UX 中的图像的 URL (相对于 CDN 基本)             |
|&nbsp;&nbsp;TechnologyId      |此内容的技术的 GUID 与可选 (- 空字符串)             |
|&nbsp;&nbsp;SubjectId         |此内容的主题的 GUID 与可选 (- 空字符串)                |
|&nbsp;&nbsp;Source            |从源数组中，除了用户添加的自定义数据外，未在 UX 中专门使用的数据被标记为"租户"，并且 UX 管理区域不允许编辑任何未标记为"租户"的项。                           |
|&nbsp;&nbsp;*子类别[ ]*|Sub-Categories级别 2 以下的导航级别。 该结构与刚刚嵌套的 Category 相同。          |
|**访问群体 [ ]**             |当与类别/子类别关联的播放列表标记了各种受众时，将可以使用选择器来显示可用受众。 |         
|&nbsp;&nbsp;Id                |访问群体 GUID                                                                       |  
|&nbsp;&nbsp;名称              |访问群体显示名称                                                               |       
|**Sources [ ]**               |使用源标记内容的字符串数组，除了用户添加的自定义数据外，未在 UX 中专门使用，这些字符串被标记为"租户"，并且 UX 管理区域不允许编辑任何未标记为"租户"的内容。                                                   |  
|**Levels [ ]**               |当与类别/子类别关联的播放列表具有各种级别的标记时，将显示可用级别的选择器。             |  
|&nbsp;&nbsp;Id                |级别的 GUID                                                                          |  
|&nbsp;&nbsp;名称              |Level 的显示名称                                                                  | 
|**StatusTag [ ]**           |状态标记用于标识将在 UX 中公开的各种状态的内容。 其中一些标志将向使用者显示，一些仅向管理员显示。                                                   |  
|&nbsp;&nbsp;Id                |StatugTag 的 GUID                                                                      |  
|&nbsp;&nbsp;名称              |StatusTag 的显示名称                                                              | 
|**遥测 [ ]**            |                                                                                           |  
|&nbsp;&nbsp;AppInsightsKey    |已设置为跟踪查看器 Web 部件加载的应用见解密钥的 GUID。 管理员可以关闭整个租户的跟踪，但发送的信息是具有租户 ID 的匿名用户。有关详细信息，请参阅本部分 https://github.com/pnp/custom-learning-office-365#disabling-telemetry-collection               |  
|**版本**                   |解决方案使用版本信息向管理员指示 Web 部件已更新，还允许 Web 部件自行将自定义内容更新到清单的最新版本（如果进行了重大更改）。         | 
|&nbsp;&nbsp;清单          |清单的版本                                               |
|&nbsp;&nbsp;ManifestMinWebPart|与清单版本一起工作的 Web 部件的最低版本             |
|&nbsp;&nbsp;CurrentWebPart    |应显示在 UX 中的图像的 URL (相对于 CDN 基本)             |
|&nbsp;&nbsp;RepoURL           |更新 Web 部件说明的存储库 URL。                    |
|**内容包**             |目前不支持其他 CDN 的内容包。 内容包允许 Microsoft 建议其他 Microsoft 创建的解决方案，这些解决方案可通过预配服务进行设置，该预配服务利用 M365LP 提供内容，并且它们本身是自定义 CDN。       | 
|&nbsp;&nbsp;Id                |内容包/CDN 的 GUID                                                              |
|&nbsp;&nbsp;名称              |CDN 的显示名称                                                                   |
|&nbsp;&nbsp;说明       |要显示在 UI 中用于添加内容包的说明                               |
|&nbsp;&nbsp;图像             |要显示在 UI 中以添加内容包的图像                                     |
|&nbsp;&nbsp;ProvisionURL      |用于创建内容包的网站集的预配服务包的 URL  |
|&nbsp;&nbsp;CDNbase           |内容包清单的基 URL                                       |
|AssetOrigins                  |在稍后介绍的 on 文件上assets.jsURL 源的数组。 如果源 URL 支持，则向用户发送一条help_getClientHeight。 data 属性中"help_getClientHeight={height of content}"的响应 (例如"help_getClientHeight=5769") 将允许 iFrame 调整为框架内容的适当高度。         |

### <a name="playlistsjson-structure"></a>Playlists.js结构
playlists.js- 播放列表清单是一组对象，用于描述播放列表的元数据和播放列表中包含的资产。

|              名称        |                     说明                                                               | 
|:-----------------------------|-------------------------------------------------------------------------------------------|
|Id                            |表示播放列表的 GUID                                                             |  
|标题                         |播放列表的显示名称                                                               |
|图像                         |相对于 URL (CDN) 图像以可视化播放列表                              |                      
|LevelId                       |关联级别                                                                           |
|AudienceId                   |关联的访问群体                                                                        |
|TechnologyId                 |关联技术                                                                      |
|SubjectId                    |类别/子类别的显示名称                                                  |
|源                        |从源数组中，除了用户添加的自定义数据外，未在 UX 中专门使用的数据被标记为"租户"，并且 UX 管理区域不允许编辑任何未标记为"租户"的项。                                              |
|CatId                         |表示应显示播放列表的容器的 Category 或 SubCategory ID。 当前，清单不支持选择 Category 或 SubCategory 作为容器（如果它还具有 SubCategory 子级）。        |
|Description                   |针对 UX 中每个播放列表显示的描述                                           |
|StatusTagId                   |关联的状态标记                                                                      |
|StatusNote                    |有关向管理员显示的内容的注释                                            |
|*Assets[]*                        |此播放列表中资产的 GUID 数组，按显示顺序显示。        |         

### <a name="assetjson-structure"></a>Asset.js结构
playlists.js- 播放列表清单是一组对象，用于描述播放列表的元数据和播放列表中包含的资产。

|              名称        |                     说明                                                               | 
|:-----------------------------|-------------------------------------------------------------------------------------------|
|Id                            |表示播放列表的 GUID                                                             |  
|标题                         |播放列表的显示名称                                                               |
|Description                   |---                                                                                           |                      
|URL                           |要应用于 iFrame 的资产的源 URL                                  |
|TechnologyId                  |关联技术                                                                      |
|SubjectId                     |关联主题                                                                         |
|源                        |类别/子类别的显示名称                                                  |
|StatusTagId                   |关联的状态标记                                                                      |
|StatusNote                    |有关向管理员显示的内容的注释。                                           |

### <a name="caching"></a>缓存
当前版本的查看器 Web 部件利用清单文件的缓存版本 24 小时。 24 小时后，第一个点击 Web 部件的用户通过从源 CDN 下载清单，将该信息与隐藏技术和播放列表合并，以及合并自定义子类别、播放列表和资产来刷新缓存的性能。 或者，管理员 Web 部件始终从清单下载内容，然后将它们合并并更新缓存。  换句话说，管理员可通过加载管理 Web 部件（即"管理"页）随时强制更新缓存。

## <a name="content-pack-guidelines"></a>内容包指南
内容包功能可解锁以下方案：
- 合作伙伴能够重新分发针对客户环境定制的增值自定义学习内容
- 具有强大培训团队和 IT 支持的组织构建面向自身内部系统和治理的自定义学习内容的能力
- Microsoft 在未来提供客户可以选择加入的其他学习路径的能力

由于此功能的复杂性，此当前文档集有意面向合作伙伴。 服务团队将积极致力于在未来更好地支持和启用#2方案。 

### <a name="how-content-packs-work"></a>内容包如何工作
Microsoft 将 GitHub 页面用作内容交付网络 (CDN) 清单文件和图像的源。 我们在 GitHub 存储库的根目录下有一个 docs 文件夹，其中包含每个版本的清单文件的子文件夹。 每个文件夹内有三个清单文件，以及一个图像文件夹，用于存储所有类别、子类别和播放列表图像。 

如果你选择使用自己的内容包扩展学习路径解决方案，则保持与 Microsoft 相同的版本控制结构非常重要。 CDN 终结点不应包含版本文件夹，因为 Web 部件支持的清单版本已放入其中，并自动追加到 CDN URL。 我们显然将给你一些时间，每次我们修订清单文件时创建清单文件的新实例。

![屏幕截图显示了示例结构。](media/cg-part-json-folder.png) 

有关将 GitHub 页面用作 CDN 源的详细信息，请参阅以下帮助文档： [https://help.github.com/en/articles/configuring-a-publishing-source-for-github-pages](https://help.github.com/en/articles/configuring-a-publishing-source-for-github-pages) 。

Microsoft 的解决方案公开有关资产的信息，因为对于谁有权访问这些文件没有任何安全性。 我们认为，应该为消费者提供一个免费的内容层，也就是说，如果你需要支付部分或所有内容费用，则需要在解决方案的技术限制内以不同方式实现这一点，并且使用 GitHub 页面不是一项要求。 如果你保持我们列出的版本编号结构，则任何希望使用的 CDN 提供商都正常。 如前所述，Web 部件支持的清单结构版本将融入代码中，并自动追加到 CDN URL。 

### <a name="content-pack-integration-guidance"></a>内容包集成指南 
管理员和查看器 Web 部件已扩展，以允许消费者在租户中配置其他 CDN 终结点，然后允许查看器 Web 部件选择应源显示数据的 CDN。 

要记住此功能的关键帧： 
- 这主要适用于合作伙伴重新分发方案 - 其中手动播放列表配置过于麻烦 
- 自定义内容包是一项高级功能，应仅由具有管理 Web 内容经验的合作伙伴使用。 不受信任的内容源可能会将不安全的内容引入您的网站。 只应添加信任的源。

> **重要** 在添加自定义内容包之前，你必须已预配 Microsoft 365 学习路径 3.0 或更高版本。 有关预配 Microsoft 365 学习路径的介绍，请参阅预配 [Microsoft 365 学习路径](./custom_provision.md)。

### <a name="content-whitelisting"></a>内容白名单
作为合作伙伴，你有责任帮助消费者确保你的内容已列入其环境中白名单。 我们建议你在你的环境中创建一个测试方案，以验证你的内容是否可放入防火墙内的 SharePoint 页面中。 按照 [创建自定义播放列表的 SharePoint 页面](./custom_createnewpage.md) 说明确认这是这种情况。

### <a name="add-a-content-pack-to-learning-pathways"></a>将内容包添加到学习路径
创建修改 JSON 并定义 CDN 后，你可以添加联系人包以学习路径。 

1. 从学习路径网站 **主页中**，指向"主页 **"，然后单击**"**学习路径管理"。** 
2. 在" **管理"** 页中，单击 **...在页面** 右上角添加内容包。
3. 单击"自定义内容包"，然后输入内容包的名称，然后指定 JSON 文件所在的 CDN。

   ![输入名称和路径的屏幕。](media/cg-part-addconpack.png)

4. 单击“保存”。 自定义内容包中的内容现在应显示在"管理"页中。 下面是一个示例。 

   ![管理页示例。](media/cg-part-addconpackex.png)

### <a name="filter-to-the-content-pack-in-the-web-part"></a>筛选到 Web 部件中的内容包
借助学习路径，你可以将学习路径 Web 部件添加到页面，筛选 Web 部件以指向自定义内容包源，然后将 Web 部件筛选为你需要的类别、子类别、播放列表和资产。 

1. 从学习路径网站中，单击 **"新建"，** 然后单击"**页面"。**
2. 单击 **"空白**"，然后单击"**创建页面"。**
3. 为页面命名。 
4. 单击 **页面左侧的" +** 添加新节"。
5. 单击 **+** 新部分的顶部中间，然后添加 **Microsoft 365 学习** 路径 Web 部件。
6. 单击 Web 部件，然后单击"编辑 **"** 图标。
7. 在 **"选择学习源** "框中，选择自定义内容包，然后将 Web 部件筛选为您想要的内容。 下面提供了从自定义内容包筛选到播放列表的 Web 部件示例。

   ![从自定义内容包中筛选到播放列表的示例 Web 部件屏幕截图。](media/cg-part-conpackfilter.png)