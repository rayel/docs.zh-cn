---
title: System.Math 方法
ms.date: 03/30/2017
ms.assetid: 0f299521-6f41-4720-bd70-67c93fc50948
ms.openlocfilehash: 8d0ac9e9eb394deaa9dcab1a276e3ef00e2ac01b
ms.sourcegitcommit: 3d5d33f384eeba41b2dff79d096f47ccc8d8f03d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/04/2018
ms.locfileid: "33357111"
---
# <a name="systemmath-methods"></a>System.Math 方法
[!INCLUDE[vbtecdlinq](../../../../../../includes/vbtecdlinq-md.md)] 不支持以下 <xref:System.Math> 方法。  
  
-   <xref:System.Math.DivRem%28System.Int32%2CSystem.Int32%2CSystem.Int32%40%29?displayProperty=nameWithType>  
  
-   <xref:System.Math.DivRem%28System.Int64%2CSystem.Int64%2CSystem.Int64%40%29?displayProperty=nameWithType>  
  
-   <xref:System.Math.IEEERemainder%28System.Double%2CSystem.Double%29?displayProperty=nameWithType>  
  
## <a name="differences-from-net"></a>与 .NET 的差异  
 .NET Framework 在舍入语义方面与 SQL Server 不同。 <xref:System.Math.Round%2A> .NET Framework 中的方法执行*银行家舍入法*，其中以.5 结尾的数字舍入到最近的偶数位而不是到下一个更高版本的数字。 例如，2.5 舍入为 2，而 3.5 则舍入为 4。 （此方法有助于避免大型数据事务中趋向较高值的系统性偏差。）  
  
 而在 SQL 中，`ROUND` 函数则始终向远离 0 的方向舍入。 因此 2.5 舍入为 3，相比之下，它在 .NET Framework 中则舍入为 2。  
  
 [!INCLUDE[vbtecdlinq](../../../../../../includes/vbtecdlinq-md.md)] 遵照 SQL `ROUND` 语义，因而不会尝试执行“四舍六入五成双”。  
  
## <a name="see-also"></a>请参阅  
 [数据类型和函数](../../../../../../docs/framework/data/adonet/sql/linq/data-types-and-functions.md)
