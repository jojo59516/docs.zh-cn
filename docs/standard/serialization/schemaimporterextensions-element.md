---
title: '&lt;schemaImporterExtensions&gt; 元素'
ms.date: 03/30/2017
helpviewer_keywords:
- XML serialization, configuration
- schemaImporterExtensions element
- <schemaImporterExtensions> element
ms.assetid: 465ef2a0-f909-4ac1-9a56-0ead5c849698
ms.openlocfilehash: c9f4f6800c2718c3b2c2b9b5b2b6d97e1114dbcb
ms.sourcegitcommit: 3d5d33f384eeba41b2dff79d096f47ccc8d8f03d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/04/2018
---
# <a name="ltschemaimporterextensionsgt-element"></a>&lt;schemaImporterExtensions&gt; 元素
包含将 XSD 类型映射到 .NET Framework 类型时 <xref:System.Xml.Serialization.XmlSchemaImporter> 所用的类型。 有关配置文件的详细信息，请参阅[配置文件架构](../../../docs/framework/configure-apps/file-schema/index.md)。  
  
## <a name="syntax"></a>语法  
  
```xml  
<schemaImporterExtensions>  
    <!-- Add types -->  
</SchemaImporterExtension>  
```  
  
## <a name="child-elements"></a>子元素  
  
|元素|描述|  
|-------------|-----------------|  
|[\<xmlSchemaImporterExtensions> 的 \<add> 元素](../../../docs/standard/serialization/add-element-for-xmlschemaimporterextensions.md)|添加 <xref:System.Xml.Serialization.XmlSchemaImporter> 用来创建映射的类型。|  
  
## <a name="parent-elements"></a>父元素  
  
|元素|描述|  
|-------------|-----------------|  
|[\<system.xml.serialization> 元素](../../../docs/standard/serialization/system-xml-serialization-element.md)|用于控制 XML 序列化的顶级元素。|  
  
## <a name="example"></a>示例  
 下面的代码示例演示如何添加将 XSD 类型映射到 .NET Framework 类型时 <xref:System.Xml.Serialization.XmlSchemaImporter> 所用的类型。  
  
```xml  
<system.xml.serialization>  
    <schemaImporterExtensions>  
        <add name = "MobileCapabilities" type =   
        "System.Web.Mobile.MobileCapabilities,   
        System.Web.Mobile, Version - 2.0.0.0, Culture = neutral,   
        PublicKeyToken = b03f5f6f11d40a3a" />  
    </schemaImporterExtensions>  
/system.sxml.serializaiton>  
```  
  
## <a name="see-also"></a>请参阅  
 <xref:System.Xml.Serialization.XmlSchemaImporter>  
 <xref:System.Xml.Serialization.Configuration.DateTimeSerializationSection.DateTimeSerializationMode>  
 [配置文件架构](../../../docs/framework/configure-apps/file-schema/index.md)  
 [\<dateTimeSerialization> 元素](../../../docs/standard/serialization/datetimeserialization-element.md)  
 [\<xmlSchemaImporterExtensions> 的 \<add> 元素](../../../docs/standard/serialization/add-element-for-xmlschemaimporterextensions.md)  
 [\<system.xml.serialization> 元素](../../../docs/standard/serialization/system-xml-serialization-element.md)
