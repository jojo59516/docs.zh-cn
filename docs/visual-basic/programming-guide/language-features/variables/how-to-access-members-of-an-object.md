---
title: 如何：访问对象的成员 (Visual Basic)
ms.date: 07/20/2015
helpviewer_keywords:
- members [Visual Basic], accessing
- object variables [Visual Basic], accessing members
ms.assetid: a0072514-6a79-4dd6-8d03-ca8c13e61ddc
ms.openlocfilehash: 62be2955bd1f62fa5af4e54fb0af5e7dca29c421
ms.sourcegitcommit: 3d5d33f384eeba41b2dff79d096f47ccc8d8f03d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/04/2018
---
# <a name="how-to-access-members-of-an-object-visual-basic"></a>如何：访问对象的成员 (Visual Basic)
如果必须引用的对象的对象变量，你通常想要使用该对象，如其方法、 属性、 字段和事件的成员。 例如，一旦你创建一个新<xref:System.Windows.Forms.Form>对象，你可能想要设置其<xref:System.Windows.Forms.Control.Text%2A>属性或调用其<xref:System.Windows.Forms.Control.Focus%2A>方法。  
  
## <a name="accessing-members"></a>成员访问  
 通过对引用该变量访问的对象的成员。  
  
#### <a name="to-access-members-of-an-object"></a>若要访问的对象的成员  
  
-   使用成员访问运算符 (`.`) 之间的对象变量名称和成员名称。  
  
    ```  
    currentText = newForm.Text  
    ```  
  
     如果该成员是[共享](../../../../visual-basic/language-reference/modifiers/shared.md)，不需要一个变量来访问它。  
  
## <a name="accessing-members-of-an-object-of-known-type"></a>已知类型的对象的成员访问  
 如果在编译时知道对象的类型，则可以使用*早期绑定*它引用的变量。  
  
#### <a name="to-access-members-of-an-object-for-which-you-know-the-type-at-compile-time"></a>若要访问的对象，您知道类型在编译时的成员  
  
1.  将你想要分配给变量对象的类型的对象变量声明。  
  
    ```  
    Dim extraForm As System.Windows.Forms.Form  
    ```  
  
     与`Option Strict On`，你可以仅分配<xref:System.Windows.Forms.Form>对象 (或类型的对象派生自<xref:System.Windows.Forms.Form>) 到`extraForm`。 如果已定义类或结构具有扩大`CType`转换为<xref:System.Windows.Forms.Form>，也可以分配该类或结构`extraForm`。  
  
2.  使用成员访问运算符 (`.`) 之间的对象变量名称和成员名称。  
  
    ```  
    extraForm.Show()  
    ```  
  
     你可以访问所有的方法和属性特定于<xref:System.Windows.Forms.Form>类，无论`Option Strict`设置。  
  
## <a name="accessing-members-of-an-object-of-unknown-type"></a>未知类型的对象的成员访问  
 如果在编译时不知道对象的类型，则必须使用*后期绑定*它是指任何变量。  
  
#### <a name="to-access-members-of-an-object-for-which-you-do-not-know-the-type-at-compile-time"></a>若要访问的对象，你不知道类型在编译时的成员  
  
1.  声明对象变量为[Object 数据类型](../../../../visual-basic/language-reference/data-types/object-data-type.md)。 (声明一个变量，作为`Object`等同于其声明为<xref:System.Object?displayProperty=nameWithType>。)  
  
    ```  
    Dim someControl As Object  
    ```  
  
     与`Option Strict On`，你可以访问仅定义的成员<xref:System.Object>类。  
  
2.  使用成员访问运算符 (`.`) 之间的对象变量名称和成员名称。  
  
    ```  
    someControl.GetType()  
    ```  
  
     若要能够访问分配给对象变量的任何对象的成员，必须设置`Option Strict Off`。 执行此操作时，编译器无法保证，由你分配给变量的对象公开给定的成员。 如果该对象未公开的成员尝试访问，<xref:System.MemberAccessException>则会发生异常。  
  
## <a name="see-also"></a>请参阅  
 <xref:System.Object>  
 <xref:System.Windows.Forms.Form>  
 <xref:System.MemberAccessException>  
 [对象变量](../../../../visual-basic/programming-guide/language-features/variables/object-variables.md)  
 [对象变量声明](../../../../visual-basic/programming-guide/language-features/variables/object-variable-declaration.md)  
 [Object 数据类型](../../../../visual-basic/language-reference/data-types/object-data-type.md)  
 [Option Strict 语句](../../../../visual-basic/language-reference/statements/option-strict-statement.md)
