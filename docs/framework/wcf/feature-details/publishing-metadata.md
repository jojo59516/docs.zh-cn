---
title: 发布元数据
ms.date: 03/30/2017
helpviewer_keywords:
- meatadata [WCF], publishing
ms.assetid: 3a56831a-cabc-45c0-bd02-12e2e9bd7313
ms.openlocfilehash: 6e6c6d10eb0cd03ea2665f1787dba4e09528a141
ms.sourcegitcommit: 3d5d33f384eeba41b2dff79d096f47ccc8d8f03d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/04/2018
---
# <a name="publishing-metadata"></a>发布元数据
Windows Communication Foundation (WCF) 服务通过发布一个或多个元数据终结点发布元数据。 发布服务元数据之后，可以通过标准协议（如 WS-MetadataExchange (MEX) 和 HTTP/GET 请求）来使用该元数据。 元数据终结点类似于其他服务终结点，因为它们都有一个地址、一个绑定和一个协定，并且它们都可通过配置或命令代码添加到服务主机。  
  
## <a name="publishing-metadata-endpoints"></a>发布元数据终结点  
 若要发布的 WCF 服务的元数据终结点，首先必须添加<xref:System.ServiceModel.Description.ServiceMetadataBehavior>服务到服务的行为。 添加一个 <xref:System.ServiceModel.Description.ServiceMetadataBehavior?displayProperty=nameWithType> 实例将允许服务公开元数据终结点。 添加 <xref:System.ServiceModel.Description.ServiceMetadataBehavior?displayProperty=nameWithType> 服务行为之后，就可以公开支持 MEX 协议或响应 HTTP/GET 请求的元数据终结点。  
  
 <xref:System.ServiceModel.Description.ServiceMetadataBehavior?displayProperty=nameWithType> 使用 <xref:System.ServiceModel.Description.WsdlExporter> 来导出服务中所有服务终结点的元数据。 有关从服务中导出元数据的详细信息，请参阅[导出和导入元数据](../../../../docs/framework/wcf/feature-details/exporting-and-importing-metadata.md)。  
  
 <xref:System.ServiceModel.Description.ServiceMetadataBehavior?displayProperty=nameWithType> 添加一个 <xref:System.ServiceModel.Description.ServiceMetadataExtension> 实例作为服务主机的扩展。 <xref:System.ServiceModel.Description.ServiceMetadataExtension?displayProperty=nameWithType> 提供了元数据发布协议的实现。 还可以使用 <xref:System.ServiceModel.Description.ServiceMetadataExtension?displayProperty=nameWithType> 通过访问 <xref:System.ServiceModel.Description.ServiceMetadataExtension.Metadata%2A?displayProperty=nameWithType> 属性来在运行时获取服务的元数据。  
  
### <a name="mex-metadata-endpoints"></a>MEX 元数据终结点  
 要添加使用 MEX 协议的元数据终结点，请将服务终结点添加到使用 `IMetadataExchange` 服务协定的服务主机。 WCF 包含<xref:System.ServiceModel.Description.IMetadataExchange>可以作为 WCF 编程模型的一部分使用此服务协定名称的接口。 Ws-metadataexchange 终结点或 MEX 终结点，可以使用在静态工厂方法公开的四种默认绑定之一<xref:System.ServiceModel.Description.MetadataExchangeBindings>类以匹配由 Svcutil.exe 之类的 WCF 工具使用的默认绑定。 还可以使用自己的自定义绑定来配置 MEX 元数据终结点。  
  
### <a name="http-get-metadata-endpoints"></a>HTTP GET 元数据终结点  
 若要将元数据终结点添加到响应 HTTP/GET 请求的服务，请将 <xref:System.ServiceModel.Description.ServiceMetadataBehavior.HttpGetEnabled%2A> 的 <xref:System.ServiceModel.Description.ServiceMetadataBehavior?displayProperty=nameWithType> 属性设置为 `true`。 将 <xref:System.ServiceModel.Description.ServiceMetadataBehavior.HttpsGetEnabled%2A> 的 <xref:System.ServiceModel.Description.ServiceMetadataBehavior?displayProperty=nameWithType> 属性设置为 `true` 还可以配置使用 HTTPS 的元数据终结点。  
  
## <a name="in-this-section"></a>本节内容  
 [如何：使用配置文件发布服务的元数据](../../../../docs/framework/wcf/feature-details/how-to-publish-metadata-for-a-service-using-a-configuration-file.md)  
 演示如何配置 WCF 服务来发布元数据，使客户端可以检索使用 Ws-metadataexchange 或 HTTP/GET 请求使用的元数据`?wsdl`查询字符串。  
  
 [如何：使用代码发布服务的元数据](../../../../docs/framework/wcf/feature-details/how-to-publish-metadata-for-a-service-using-code.md)  
 演示如何启用代码中的 WCF 服务的元数据发布，以便客户端能够检索使用 Ws-metadataexchange 或 HTTP/GET 请求使用的元数据`?wsdl`查询字符串。  
  
## <a name="reference"></a>参考  
 <xref:System.ServiceModel.Description.ServiceMetadataBehavior>  
  
 <xref:System.ServiceModel.Description.IMetadataExchange>  
  
 <xref:System.ServiceModel.Description.ServiceMetadataExtension>  
  
 <xref:System.ServiceModel.Description.MetadataExchangeBindings>  
  
## <a name="see-also"></a>请参阅  
 [导出和导入元数据](../../../../docs/framework/wcf/feature-details/exporting-and-importing-metadata.md)
