---
title: '&lt;删除&gt;元素&lt;namedCaches&gt;'
ms.date: 03/30/2017
helpviewer_keywords:
- remove element for namedCaches
- <remove> element for namedCaches
ms.assetid: 24211ea5-163e-4fe5-aed8-004d8499760c
author: mcleblanc
ms.author: markl
manager: markl
ms.openlocfilehash: 6ffaea24910a6b8f4a120d6b72219bff592fab17
ms.sourcegitcommit: 11f11ca6cefe555972b3a5c99729d1a7523d8f50
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/03/2018
---
# <a name="ltremovegt-element-for-ltnamedcachesgt"></a>&lt;删除&gt;元素&lt;namedCaches&gt;
从内存缓存的 `namedCaches` 集合中删除一个命名的缓存条目。  
  
 \<system.runtime.caching>  
\<memoryCache>  
\<namedCaches >  
\<remove>  
  
## <a name="syntax"></a>语法  
  
```xml  
<namedCaches>  
    <remove name="default" />  
    <!-- child elements -->  
 </namedCaches>  
```  
  
## <a name="type"></a>类型  
 `None`  
  
## <a name="attributes-and-elements"></a>特性和元素  
 下列各节描述了特性、子元素和父元素。  
  
### <a name="attributes"></a>特性  
 `None`  
  
### <a name="child-elements"></a>子元素  
 `None`  
  
### <a name="parent-elements"></a>父元素  
  
|元素|描述|  
|-------------|-----------------|  
|[\<namedCaches>](../../../../../docs/framework/configure-apps/file-schema/runtime/namedcaches-element-cache-settings.md)|包含的配置设置的命名集合<xref:System.Runtime.Caching.MemoryCache>实例。|  
  
## <a name="remarks"></a>备注  
 `remove`元素中删除`namedCache`内存缓存的命名的缓存集合中的条目。  
  
## <a name="see-also"></a>请参阅  
 [\<namedCaches > 元素 （缓存设置）](../../../../../docs/framework/configure-apps/file-schema/runtime/namedcaches-element-cache-settings.md)
