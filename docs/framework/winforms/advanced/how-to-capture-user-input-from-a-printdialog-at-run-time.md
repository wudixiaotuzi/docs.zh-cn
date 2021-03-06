---
title: 如何：在运行时从 PrintDialog 中捕获用户输入
ms.date: 03/30/2017
dev_langs:
- csharp
- vb
- cpp
helpviewer_keywords:
- print options [Windows Forms], changing at run time
- printing [Windows Forms], options
- print options
- run time [Windows Forms], changing print options
ms.assetid: 438501d8-9a70-4fb3-aae6-e46579aba0c6
ms.openlocfilehash: 554c3c43f8ac4d41ddfc8651472d0b7fbed960bb
ms.sourcegitcommit: 3d5d33f384eeba41b2dff79d096f47ccc8d8f03d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/04/2018
ms.locfileid: "33522871"
---
# <a name="how-to-capture-user-input-from-a-printdialog-at-run-time"></a>如何：在运行时从 PrintDialog 中捕获用户输入
尽管你可以设置与在设计时打印相关的选项，有时想要在运行时，由于用户所做选择最有可能更改这些选项。 你可以捕获有关打印文档使用的用户输入<xref:System.Windows.Forms.PrintDialog>和<xref:System.Drawing.Printing.PrintDocument>组件。  
  
### <a name="to-change-print-options-programmatically"></a>若要以编程方式更改打印选项  
  
1.  添加<xref:System.Windows.Forms.PrintDialog>和<xref:System.Drawing.Printing.PrintDocument>组件向窗体。  
  
2.  设置<xref:System.Windows.Forms.PrintDialog.Document%2A>属性<xref:System.Windows.Forms.PrintDialog>到<xref:System.Drawing.Printing.PrintDocument>添加到窗体。  
  
    ```vb  
    PrintDialog1.Document = PrintDocument1  
    ```  
  
    ```csharp  
    printDialog1.Document = PrintDocument1;  
    ```  
  
    ```cpp  
    printDialog1->Document = PrintDocument1;  
    ```  
  
3.  显示<xref:System.Windows.Forms.PrintDialog>组件使用<xref:System.Windows.Forms.CommonDialog.ShowDialog%2A>方法。  
  
    ```vb  
    PrintDialog1.ShowDialog()  
    ```  
  
    ```csharp  
    printDialog1.ShowDialog();  
    ```  
  
    ```cpp  
    printDialog1->ShowDialog();  
    ```  
  
4.  从对话框的用户的打印选项将复制到<xref:System.Drawing.Printing.PrinterSettings>属性<xref:System.Drawing.Printing.PrintDocument>组件。  
  
## <a name="see-also"></a>请参阅  
 [如何：打印 Windows 窗体中的多页文本文件](../../../../docs/framework/winforms/advanced/how-to-print-a-multi-page-text-file-in-windows-forms.md)  
 [Windows 窗体打印支持](../../../../docs/framework/winforms/advanced/windows-forms-print-support.md)
