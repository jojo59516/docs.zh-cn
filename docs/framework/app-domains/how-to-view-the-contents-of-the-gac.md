---
title: 如何：查看全局程序集缓存的内容
ms.date: 03/30/2017
helpviewer_keywords:
- assemblies [.NET Framework], global assembly cache
- global assembly cache, viewing contents
- viewing assemblies in global assembly cache
- Gacutil.exe
- strong-named assemblies, global assembly cache
- GAC (global assembly cache), viewing contents
- list of assemblies in global assembly cache
- Global Assembly Cache tool
ms.assetid: c5f786a0-969b-4f14-9f02-e77c3384d9af
author: rpetrusha
ms.author: ronpet
ms.openlocfilehash: d6e582f86eac03a51437b965f87f1bc7f29294eb
ms.sourcegitcommit: 11f11ca6cefe555972b3a5c99729d1a7523d8f50
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/03/2018
---
# <a name="how-to-view-the-contents-of-the-global-assembly-cache"></a>如何：查看全局程序集缓存的内容
使用[全局程序集缓存工具 (Gacutil.exe)](../../../docs/framework/tools/gacutil-exe-gac-tool.md) 可查看全局程序集缓存的内容。  
  
### <a name="to-view-a-list-of-the-assemblies-in-the-global-assembly-cache"></a>查看全局程序集缓存中的程序集列表  
  
1.  在 [Visual Studio 命令提示符](../../../docs/framework/tools/developer-command-prompt-for-vs.md)处，键入以下命令：  
  
     gacutil -l   
     或  
    gacutil -l  
  
 在 .NET Framework 的早期版本中，可通过 [Shfusion.dll](http://msdn.microsoft.com/library/0d9464cf-ddba-4ca9-bbec-f678fb58f380) Windows shell 扩展在文件资源管理器中查看全局程序集缓存。 从 [!INCLUDE[net_v40_long](../../../includes/net-v40-long-md.md)]开始，Shfusion.dll 已过时。  
  
## <a name="see-also"></a>请参阅  
 [使用程序集和全局程序集缓存](../../../docs/framework/app-domains/working-with-assemblies-and-the-gac.md)  
 [Gacutil.exe（全局程序集缓存工具）](../../../docs/framework/tools/gacutil-exe-gac-tool.md)
