---
title: Entity Type — 实体类型
ms.date: 03/30/2017
ms.assetid: a6dee9ab-9e4a-48f2-a169-3f79cc15821c
ms.openlocfilehash: c694f29d36988ea52aeca650cf2bba2c50c91e89
ms.sourcegitcommit: 11f11ca6cefe555972b3a5c99729d1a7523d8f50
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/03/2018
---
# <a name="entity-type"></a>Entity Type — 实体类型
*实体类型*是用于描述实体数据模型 (EDM) 的数据结构的基本构建块。 在概念模型中，实体类型表示顶级概念（例如客户或订单）的结构。 实体类型是实体类型实例的模板。 每个模板都包含以下信息：  
  
-   唯一名称。 （必选。）  
  
-   [实体键](../../../../docs/framework/data/adonet/entity-key.md)由一个或多个属性定义。 （必选。）  
  
-   形式的数据[属性](../../../../docs/framework/data/adonet/property.md)。 （可选）。  
  
-   [导航属性](../../../../docs/framework/data/adonet/navigation-property.md)，可以从一个导航[结束](../../../../docs/framework/data/adonet/association-end.md)的[关联](../../../../docs/framework/data/adonet/association-type.md)到的另一端。 （可选）  
  
 在应用程序中，实体类型的实例表示一个特定对象（例如特定客户或订单）。 实体类型的每个实例必须具有唯一[实体键](../../../../docs/framework/data/adonet/entity-key.md)内[实体集](../../../../docs/framework/data/adonet/entity-set.md)。  
  
 只有两个实体类型实例的类型相同且其实体键的值也相同时，才认为它们是相等的。  
  
## <a name="example"></a>示例  
 下图显示了一个具有三个实体类型的概念模型：`Book`、`Publisher` 和 `Author`：  
  
 ![示例模型](../../../../docs/framework/data/adonet/media/examplemodel.gif "ExampleModel")  
  
 请注意，构成其实体键的每个实体类型的属性均用“(Key)”标示出来。  
  
 [ADO.NET 实体框架](../../../../docs/framework/data/adonet/ef/index.md)使用域特定语言 (DSL) 称为概念架构定义语言 ([CSDL](../../../../docs/framework/data/adonet/ef/language-reference/csdl-specification.md)) 来定义概念模型。 下面的 CSDL 定义了上图中显示的 `Book` 实体类型。  
  
 [!code-xml[EDM_Example_Model#EntityExample](../../../../samples/snippets/xml/VS_Snippets_Data/edm_example_model/xml/books.edmx#entityexample)]  
  
## <a name="see-also"></a>请参阅  
 [实体数据模型关键概念](../../../../docs/framework/data/adonet/entity-data-model-key-concepts.md)  
 [实体数据模型](../../../../docs/framework/data/adonet/entity-data-model.md)  
 [facet](../../../../docs/framework/data/adonet/facet.md)
