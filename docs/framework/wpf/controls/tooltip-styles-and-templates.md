---
title: ToolTip 样式和模板
ms.date: 03/30/2017
helpviewer_keywords:
- parts [WPF], ToolTip
- styles [WPF], ToolTip
- states [WPF], ToolTip
- ToolTip [WPF], styles and templates
- ControlTemplate [WPF], ToolTip
- templates [WPF], ToolTip
ms.assetid: 405fe385-4de9-49ee-a448-d8f4d1f740dd
ms.openlocfilehash: 53b21f610ba957370fac70b79e6a827d624b6473
ms.sourcegitcommit: 43924acbdbb3981d103e11049bbe460457d42073
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/23/2018
ms.locfileid: "34457289"
---
# <a name="tooltip-styles-and-templates"></a>ToolTip 样式和模板
本主题介绍的样式和模板的<xref:System.Windows.Controls.ToolTip>控件。 你可以修改默认<xref:System.Windows.Controls.ControlTemplate>提供独特外观的控件。 有关详细信息，请参阅[通过创建 ControlTemplate 自定义现有控件的外观](../../../../docs/framework/wpf/controls/customizing-the-appearance-of-an-existing-control.md)。  
  
## <a name="tooltip-parts"></a>工具提示部分  
 <xref:System.Windows.Controls.ToolTip>控件不具有任何已命名的部件。  
  
## <a name="tooltip-states"></a>工具提示的状态  
 下表列出的可视状态<xref:System.Windows.Controls.ToolTip>控件。  
  
|VisualState 名称|VisualStateGroup 名称|描述|  
|-|-|-|  
|Closed|OpenStates|默认状态。|  
|打开|OpenStates|<xref:System.Windows.Controls.ToolTip>可见。|  
|有效|ValidationStates|该控件使用<xref:System.Windows.Controls.Validation>类和<xref:System.Windows.Controls.Validation.HasError%2A?displayProperty=nameWithType>附加的属性`false`。|  
|InvalidFocused|ValidationStates|<xref:System.Windows.Controls.Validation.HasError%2A?displayProperty=nameWithType>附加的属性`true`已在控件有焦点。|  
|InvalidUnfocused|ValidationStates|<xref:System.Windows.Controls.Validation.HasError%2A?displayProperty=nameWithType>附加的属性`true`具有该控件没有焦点。|  
  
## <a name="tooltip-controltemplate-example"></a>工具提示 ControlTemplate 示例  
 下面的示例演示如何定义<xref:System.Windows.Controls.ControlTemplate>为<xref:System.Windows.Controls.ToolTip>控件。  
  
 [!code-xaml[ControlTemplateExamples#ToolTip](../../../../samples/snippets/csharp/VS_Snippets_Wpf/ControlTemplateExamples/CS/resources/tooltip.xaml#tooltip)]  
  
 上一示例使用了一个或多个以下资源。  
  
 [!code-xaml[ControlTemplateExamples#Resources](../../../../samples/snippets/csharp/VS_Snippets_Wpf/ControlTemplateExamples/CS/resources/shared.xaml#resources)]  
  
 有关完整示例，请参阅[使用 ControlTemplates 设置样式示例](https://github.com/Microsoft/WPF-Samples/tree/master/Styles%20&%20Templates/IntroToStylingAndTemplating)。  
  
## <a name="see-also"></a>请参阅  
 <xref:System.Windows.FrameworkElement.Style%2A>  
 <xref:System.Windows.Controls.ControlTemplate>  
 [控件样式和模板](../../../../docs/framework/wpf/controls/control-styles-and-templates.md)  
 [控件自定义](../../../../docs/framework/wpf/controls/control-customization.md)  
 [样式设置和模板化](../../../../docs/framework/wpf/controls/styling-and-templating.md)  
 [通过创建 ControlTemplate 自定义现有控件的外观](../../../../docs/framework/wpf/controls/customizing-the-appearance-of-an-existing-control.md)
